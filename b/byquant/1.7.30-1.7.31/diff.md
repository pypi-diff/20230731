# Comparing `tmp/byquant-1.7.30.tar.gz` & `tmp/byquant-1.7.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byquant-1.7.30.tar", last modified: Sun Jul 30 04:51:22 2023, max compression
+gzip compressed data, was "byquant-1.7.31.tar", last modified: Mon Jul 31 02:52:18 2023, max compression
```

## Comparing `byquant-1.7.30.tar` & `byquant-1.7.31.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 04:51:22.990858 byquant-1.7.30/
--rw-rw-rw-   0        0        0     1451 2023-07-30 04:51:22.988864 byquant-1.7.30/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-05-16 07:39:16.000000 byquant-1.7.30/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 04:51:22.219316 byquant-1.7.30/byquant/
--rw-rw-rw-   0        0        0     7796 2023-07-30 04:46:35.000000 byquant-1.7.30/byquant/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 04:51:22.272259 byquant-1.7.30/byquant/crypto/
--rw-rw-rw-   0        0        0       63 2023-06-27 01:17:34.000000 byquant-1.7.30/byquant/crypto/__init__.py
--rw-rw-rw-   0        0        0    17167 2023-06-27 01:17:45.000000 byquant-1.7.30/byquant/crypto/broker.py
--rw-rw-rw-   0        0        0     8092 2023-06-27 01:17:57.000000 byquant-1.7.30/byquant/crypto/feed.py
--rw-rw-rw-   0        0        0     7942 2021-09-04 05:54:05.000000 byquant-1.7.30/byquant/crypto/store.py
-drwxrwxrwx   0        0        0        0 2023-07-30 04:51:22.282231 byquant-1.7.30/byquant/data/
--rw-rw-rw-   0        0        0      225 2023-07-28 10:25:11.000000 byquant-1.7.30/byquant/data/__init__.py
--rw-rw-rw-   0        0        0    25800 2023-07-28 11:41:13.000000 byquant-1.7.30/byquant/data/get.py
-drwxrwxrwx   0        0        0        0 2023-07-30 04:51:22.899904 byquant-1.7.30/byquant/exchange/
--rw-rw-rw-   0        0        0    14497 2023-07-28 11:41:17.000000 byquant-1.7.30/byquant/exchange/__init__.py
--rw-rw-rw-   0        0        0    41329 2023-05-15 07:52:05.000000 byquant-1.7.30/byquant/exchange/ace.py
--rw-rw-rw-   0        0        0    33161 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/alpaca.py
--rw-rw-rw-   0        0        0   129270 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/ascendex.py
--rw-rw-rw-   0        0        0     1136 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bequant.py
--rw-rw-rw-   0        0        0    62340 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bigone.py
--rw-rw-rw-   0        0        0   378516 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/binance.py
--rw-rw-rw-   0        0        0     1645 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/binancecoinm.py
--rw-rw-rw-   0        0        0     2151 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/binanceus.py
--rw-rw-rw-   0        0        0     2480 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/binanceusdm.py
--rw-rw-rw-   0        0        0    35482 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bit2c.py
--rw-rw-rw-   0        0        0    39008 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bitbank.py
--rw-rw-rw-   0        0        0      448 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bitbay.py
--rw-rw-rw-   0        0        0    45973 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bitbns.py
--rw-rw-rw-   0        0        0      467 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bitcoincom.py
--rw-rw-rw-   0        0        0    69312 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bitfinex.py
--rw-rw-rw-   0        0        0   111509 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bitfinex2.py
--rw-rw-rw-   0        0        0    37741 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bitflyer.py
--rw-rw-rw-   0        0        0    28316 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bitforex.py
--rw-rw-rw-   0        0        0   204946 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bitget.py
--rw-rw-rw-   0        0        0    42572 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bithumb.py
--rw-rw-rw-   0        0        0   131429 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bitmart.py
--rw-rw-rw-   0        0        0   119564 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bitmex.py
--rw-rw-rw-   0        0        0    63261 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bitopro.py
--rw-rw-rw-   0        0        0    87308 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bitpanda.py
--rw-rw-rw-   0        0        0    88097 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bitrue.py
--rw-rw-rw-   0        0        0    68449 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bitso.py
--rw-rw-rw-   0        0        0    82190 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bitstamp.py
--rw-rw-rw-   0        0        0    17785 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bitstamp1.py
--rw-rw-rw-   0        0        0    93397 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bittrex.py
--rw-rw-rw-   0        0        0    76761 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bitvavo.py
--rw-rw-rw-   0        0        0    74167 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bkex.py
--rw-rw-rw-   0        0        0    16241 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bl3p.py
--rw-rw-rw-   0        0        0    47120 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/blockchaincom.py
--rw-rw-rw-   0        0        0    35160 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/btcalpha.py
--rw-rw-rw-   0        0        0    22489 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/btcbox.py
--rw-rw-rw-   0        0        0   110784 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/btcex.py
--rw-rw-rw-   0        0        0    48547 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/btcmarkets.py
--rw-rw-rw-   0        0        0    22177 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/btctradeua.py
--rw-rw-rw-   0        0        0    35384 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/btcturk.py
--rw-rw-rw-   0        0        0    45591 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/buda.py
--rw-rw-rw-   0        0        0   393944 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/bybit.py
--rw-rw-rw-   0        0        0    64922 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/cex.py
--rw-rw-rw-   0        0        0   124582 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/coinbase.py
--rw-rw-rw-   0        0        0     1219 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/coinbaseprime.py
--rw-rw-rw-   0        0        0    73787 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/coinbasepro.py
--rw-rw-rw-   0        0        0    34208 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/coincheck.py
--rw-rw-rw-   0        0        0   191859 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/coinex.py
--rw-rw-rw-   0        0        0    38956 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/coinfalcon.py
--rw-rw-rw-   0        0        0    39461 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/coinmate.py
--rw-rw-rw-   0        0        0    34455 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/coinone.py
--rw-rw-rw-   0        0        0    81092 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/coinsph.py
--rw-rw-rw-   0        0        0    18778 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/coinspot.py
--rw-rw-rw-   0        0        0   108248 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/cryptocom.py
--rw-rw-rw-   0        0        0    79611 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/currencycom.py
--rw-rw-rw-   0        0        0    84060 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/delta.py
--rw-rw-rw-   0        0        0   119018 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/deribit.py
--rw-rw-rw-   0        0        0   152160 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/digifinex.py
--rw-rw-rw-   0        0        0    88724 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/exmo.py
--rw-rw-rw-   0        0        0     1169 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/flowbtc.py
--rw-rw-rw-   0        0        0     1238 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/fmfwio.py
--rw-rw-rw-   0        0        0   221725 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/gate.py
--rw-rw-rw-   0        0        0      445 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/gateio.py
--rw-rw-rw-   0        0        0    69001 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/gemini.py
--rw-rw-rw-   0        0        0    62241 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/hitbtc.py
--rw-rw-rw-   0        0        0   116511 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/hitbtc3.py
--rw-rw-rw-   0        0        0    69194 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/hollaex.py
--rw-rw-rw-   0        0        0   362643 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/huobi.py
--rw-rw-rw-   0        0        0    86605 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/huobijp.py
--rw-rw-rw-   0        0        0      572 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/huobipro.py
--rw-rw-rw-   0        0        0    67332 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/idex.py
--rw-rw-rw-   0        0        0    29810 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/independentreserve.py
--rw-rw-rw-   0        0        0    42437 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/indodax.py
--rw-rw-rw-   0        0        0    34960 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/itbit.py
--rw-rw-rw-   0        0        0   101404 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/kraken.py
--rw-rw-rw-   0        0        0    81722 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/krakenfutures.py
--rw-rw-rw-   0        0        0   160363 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/kucoin.py
--rw-rw-rw-   0        0        0   101171 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/kucoinfutures.py
--rw-rw-rw-   0        0        0    37750 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/kuna.py
--rw-rw-rw-   0        0        0    70007 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/latoken.py
--rw-rw-rw-   0        0        0    33717 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/lbank.py
--rw-rw-rw-   0        0        0    97857 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/lbank2.py
--rw-rw-rw-   0        0        0    40473 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/luno.py
--rw-rw-rw-   0        0        0    48461 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/lykke.py
--rw-rw-rw-   0        0        0    34639 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/mercado.py
--rw-rw-rw-   0        0        0   209226 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/mexc.py
--rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/mexc3.py
--rw-rw-rw-   0        0        0   106106 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/ndax.py
--rw-rw-rw-   0        0        0    61638 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/novadax.py
--rw-rw-rw-   0        0        0    37055 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/oceanex.py
--rw-rw-rw-   0        0        0   177794 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/okcoin.py
--rw-rw-rw-   0        0        0      434 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/okex.py
--rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/okex5.py
--rw-rw-rw-   0        0        0   264399 2023-06-15 05:48:33.000000 byquant-1.7.30/byquant/exchange/okx.py
--rw-rw-rw-   0        0        0    22745 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/paymium.py
--rw-rw-rw-   0        0        0   191805 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/phemex.py
--rw-rw-rw-   0        0        0    88311 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/poloniex.py
--rw-rw-rw-   0        0        0    75104 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/poloniexfutures.py
--rw-rw-rw-   0        0        0    69774 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/probit.py
--rw-rw-rw-   0        0        0    47325 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/ripio.py
--rw-rw-rw-   0        0        0   117868 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/stex.py
--rw-rw-rw-   0        0        0    42407 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/tidex.py
--rw-rw-rw-   0        0        0    65452 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/timex.py
--rw-rw-rw-   0        0        0   119250 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/tokocrypto.py
--rw-rw-rw-   0        0        0    75531 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/upbit.py
--rw-rw-rw-   0        0        0   103453 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/wavesexchange.py
--rw-rw-rw-   0        0        0    35544 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/wazirx.py
--rw-rw-rw-   0        0        0    92139 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/whitebit.py
--rw-rw-rw-   0        0        0    94453 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/woo.py
--rw-rw-rw-   0        0        0   196488 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/xt.py
--rw-rw-rw-   0        0        0    51368 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/yobit.py
--rw-rw-rw-   0        0        0    28777 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/zaif.py
--rw-rw-rw-   0        0        0   183857 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/zb.py
--rw-rw-rw-   0        0        0    74036 2023-05-14 16:20:52.000000 byquant-1.7.30/byquant/exchange/zonda.py
-drwxrwxrwx   0        0        0        0 2023-07-30 04:51:22.941610 byquant-1.7.30/byquant/indicator/
--rw-rw-rw-   0        0        0     1017 2023-07-28 11:52:03.000000 byquant-1.7.30/byquant/indicator/__init__.py
--rw-rw-rw-   0        0        0     1350 2023-07-30 04:04:11.000000 byquant-1.7.30/byquant/indicator/atr.py
--rw-rw-rw-   0        0        0     1424 2023-07-30 01:56:13.000000 byquant-1.7.30/byquant/indicator/bbands.py
--rw-rw-rw-   0        0        0     1350 2023-07-30 03:15:25.000000 byquant-1.7.30/byquant/indicator/cci.py
--rw-rw-rw-   0        0        0     1333 2023-07-30 01:58:37.000000 byquant-1.7.30/byquant/indicator/dema.py
--rw-rw-rw-   0        0        0     1325 2023-07-30 02:00:58.000000 byquant-1.7.30/byquant/indicator/ma.py
--rw-rw-rw-   0        0        0     1499 2023-07-30 04:04:44.000000 byquant-1.7.30/byquant/indicator/macd.py
--rw-rw-rw-   0        0        0     1319 2023-07-30 04:03:37.000000 byquant-1.7.30/byquant/indicator/rsi.py
--rw-rw-rw-   0        0        0     1314 2023-07-30 03:57:07.000000 byquant-1.7.30/byquant/indicator/sma.py
-drwxrwxrwx   0        0        0        0 2023-07-30 04:51:22.967308 byquant-1.7.30/byquant/indicators/
--rw-rw-rw-   0        0        0     1017 2023-07-28 11:52:03.000000 byquant-1.7.30/byquant/indicators/__init__.py
--rw-rw-rw-   0        0        0     1253 2023-07-30 04:22:54.000000 byquant-1.7.30/byquant/indicators/atr.py
--rw-rw-rw-   0        0        0     1253 2023-07-30 04:22:48.000000 byquant-1.7.30/byquant/indicators/cci.py
--rw-rw-rw-   0        0        0     1254 2023-07-30 04:22:40.000000 byquant-1.7.30/byquant/indicators/macd.py
--rw-rw-rw-   0        0        0     1254 2023-07-30 04:22:36.000000 byquant-1.7.30/byquant/indicators/rsi.py
--rw-rw-rw-   0        0        0     1254 2023-07-30 04:24:59.000000 byquant-1.7.30/byquant/indicators/sma.py
--rw-rw-rw-   0        0        0     1117 2023-07-30 04:29:44.000000 byquant-1.7.30/byquant/metastrategy.py
-drwxrwxrwx   0        0        0        0 2023-07-30 04:51:22.974149 byquant-1.7.30/byquant/strategy/
--rw-rw-rw-   0        0        0      922 2023-07-30 04:49:12.000000 byquant-1.7.30/byquant/strategy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 04:51:22.982128 byquant-1.7.30/byquant/tool/
--rw-rw-rw-   0        0        0        0 2023-06-27 01:25:40.000000 byquant-1.7.30/byquant/tool/__init__.py
--rw-rw-rw-   0        0        0     3427 2023-02-15 05:30:28.000000 byquant-1.7.30/byquant/tool/tawPlus.py
-drwxrwxrwx   0        0        0        0 2023-07-30 04:51:22.249997 byquant-1.7.30/byquant.egg-info/
--rw-rw-rw-   0        0        0     1451 2023-07-30 04:51:22.000000 byquant-1.7.30/byquant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4055 2023-07-30 04:51:22.000000 byquant-1.7.30/byquant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 04:51:22.000000 byquant-1.7.30/byquant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-07-30 04:51:22.000000 byquant-1.7.30/byquant.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-30 04:51:22.000000 byquant-1.7.30/byquant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-15 09:08:59.000000 byquant-1.7.30/byquant.egg-info/zip-safe
--rw-rw-rw-   0        0        0      190 2023-07-30 04:50:46.000000 byquant-1.7.30/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-30 04:51:22.990858 byquant-1.7.30/setup.cfg
--rw-rw-rw-   0        0        0     2880 2023-07-30 04:50:52.000000 byquant-1.7.30/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:52:18.975697 byquant-1.7.31/
+-rw-rw-rw-   0        0        0     1451 2023-07-31 02:52:18.975697 byquant-1.7.31/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-05-16 07:39:16.000000 byquant-1.7.31/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 02:52:18.163145 byquant-1.7.31/byquant/
+-rw-rw-rw-   0        0        0     7796 2023-07-30 04:46:35.000000 byquant-1.7.31/byquant/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:52:18.210022 byquant-1.7.31/byquant/crypto/
+-rw-rw-rw-   0        0        0       63 2023-06-27 01:17:34.000000 byquant-1.7.31/byquant/crypto/__init__.py
+-rw-rw-rw-   0        0        0    17167 2023-06-27 01:17:45.000000 byquant-1.7.31/byquant/crypto/broker.py
+-rw-rw-rw-   0        0        0     8092 2023-06-27 01:17:57.000000 byquant-1.7.31/byquant/crypto/feed.py
+-rw-rw-rw-   0        0        0     7942 2021-09-04 05:54:05.000000 byquant-1.7.31/byquant/crypto/store.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:52:18.217999 byquant-1.7.31/byquant/data/
+-rw-rw-rw-   0        0        0      225 2023-07-28 10:25:11.000000 byquant-1.7.31/byquant/data/__init__.py
+-rw-rw-rw-   0        0        0    25800 2023-07-28 11:41:13.000000 byquant-1.7.31/byquant/data/get.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:52:18.808341 byquant-1.7.31/byquant/exchange/
+-rw-rw-rw-   0        0        0    14497 2023-07-28 11:41:17.000000 byquant-1.7.31/byquant/exchange/__init__.py
+-rw-rw-rw-   0        0        0    41329 2023-05-15 07:52:05.000000 byquant-1.7.31/byquant/exchange/ace.py
+-rw-rw-rw-   0        0        0    33161 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/alpaca.py
+-rw-rw-rw-   0        0        0   129270 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/ascendex.py
+-rw-rw-rw-   0        0        0     1136 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bequant.py
+-rw-rw-rw-   0        0        0    62340 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bigone.py
+-rw-rw-rw-   0        0        0   378516 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/binance.py
+-rw-rw-rw-   0        0        0     1645 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/binancecoinm.py
+-rw-rw-rw-   0        0        0     2151 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/binanceus.py
+-rw-rw-rw-   0        0        0     2480 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/binanceusdm.py
+-rw-rw-rw-   0        0        0    35482 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bit2c.py
+-rw-rw-rw-   0        0        0    39008 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bitbank.py
+-rw-rw-rw-   0        0        0      448 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bitbay.py
+-rw-rw-rw-   0        0        0    45973 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bitbns.py
+-rw-rw-rw-   0        0        0      467 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bitcoincom.py
+-rw-rw-rw-   0        0        0    69312 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bitfinex.py
+-rw-rw-rw-   0        0        0   111509 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bitfinex2.py
+-rw-rw-rw-   0        0        0    37741 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bitflyer.py
+-rw-rw-rw-   0        0        0    28316 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bitforex.py
+-rw-rw-rw-   0        0        0   204946 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bitget.py
+-rw-rw-rw-   0        0        0    42572 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bithumb.py
+-rw-rw-rw-   0        0        0   131429 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bitmart.py
+-rw-rw-rw-   0        0        0   119564 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bitmex.py
+-rw-rw-rw-   0        0        0    63261 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bitopro.py
+-rw-rw-rw-   0        0        0    87308 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bitpanda.py
+-rw-rw-rw-   0        0        0    88097 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bitrue.py
+-rw-rw-rw-   0        0        0    68449 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bitso.py
+-rw-rw-rw-   0        0        0    82190 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bitstamp.py
+-rw-rw-rw-   0        0        0    17785 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bitstamp1.py
+-rw-rw-rw-   0        0        0    93397 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bittrex.py
+-rw-rw-rw-   0        0        0    76761 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bitvavo.py
+-rw-rw-rw-   0        0        0    74167 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bkex.py
+-rw-rw-rw-   0        0        0    16241 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bl3p.py
+-rw-rw-rw-   0        0        0    47120 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/blockchaincom.py
+-rw-rw-rw-   0        0        0    35160 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/btcalpha.py
+-rw-rw-rw-   0        0        0    22489 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/btcbox.py
+-rw-rw-rw-   0        0        0   110784 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/btcex.py
+-rw-rw-rw-   0        0        0    48547 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/btcmarkets.py
+-rw-rw-rw-   0        0        0    22177 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/btctradeua.py
+-rw-rw-rw-   0        0        0    35384 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/btcturk.py
+-rw-rw-rw-   0        0        0    45591 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/buda.py
+-rw-rw-rw-   0        0        0   393944 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/bybit.py
+-rw-rw-rw-   0        0        0    64922 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/cex.py
+-rw-rw-rw-   0        0        0   124582 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/coinbase.py
+-rw-rw-rw-   0        0        0     1219 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/coinbaseprime.py
+-rw-rw-rw-   0        0        0    73787 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/coinbasepro.py
+-rw-rw-rw-   0        0        0    34208 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/coincheck.py
+-rw-rw-rw-   0        0        0   191859 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/coinex.py
+-rw-rw-rw-   0        0        0    38956 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/coinfalcon.py
+-rw-rw-rw-   0        0        0    39461 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/coinmate.py
+-rw-rw-rw-   0        0        0    34455 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/coinone.py
+-rw-rw-rw-   0        0        0    81092 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/coinsph.py
+-rw-rw-rw-   0        0        0    18778 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/coinspot.py
+-rw-rw-rw-   0        0        0   108248 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/cryptocom.py
+-rw-rw-rw-   0        0        0    79611 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/currencycom.py
+-rw-rw-rw-   0        0        0    84060 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/delta.py
+-rw-rw-rw-   0        0        0   119018 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/deribit.py
+-rw-rw-rw-   0        0        0   152160 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/digifinex.py
+-rw-rw-rw-   0        0        0    88724 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/exmo.py
+-rw-rw-rw-   0        0        0     1169 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/flowbtc.py
+-rw-rw-rw-   0        0        0     1238 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/fmfwio.py
+-rw-rw-rw-   0        0        0   221725 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/gate.py
+-rw-rw-rw-   0        0        0      445 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/gateio.py
+-rw-rw-rw-   0        0        0    69001 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/gemini.py
+-rw-rw-rw-   0        0        0    62241 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/hitbtc.py
+-rw-rw-rw-   0        0        0   116511 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/hitbtc3.py
+-rw-rw-rw-   0        0        0    69194 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/hollaex.py
+-rw-rw-rw-   0        0        0   362643 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/huobi.py
+-rw-rw-rw-   0        0        0    86605 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/huobijp.py
+-rw-rw-rw-   0        0        0      572 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/huobipro.py
+-rw-rw-rw-   0        0        0    67332 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/idex.py
+-rw-rw-rw-   0        0        0    29810 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/independentreserve.py
+-rw-rw-rw-   0        0        0    42437 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/indodax.py
+-rw-rw-rw-   0        0        0    34960 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/itbit.py
+-rw-rw-rw-   0        0        0   101404 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/kraken.py
+-rw-rw-rw-   0        0        0    81722 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/krakenfutures.py
+-rw-rw-rw-   0        0        0   160363 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/kucoin.py
+-rw-rw-rw-   0        0        0   101171 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/kucoinfutures.py
+-rw-rw-rw-   0        0        0    37750 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/kuna.py
+-rw-rw-rw-   0        0        0    70007 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/latoken.py
+-rw-rw-rw-   0        0        0    33717 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/lbank.py
+-rw-rw-rw-   0        0        0    97857 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/lbank2.py
+-rw-rw-rw-   0        0        0    40473 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/luno.py
+-rw-rw-rw-   0        0        0    48461 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/lykke.py
+-rw-rw-rw-   0        0        0    34639 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/mercado.py
+-rw-rw-rw-   0        0        0   209226 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/mexc.py
+-rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/mexc3.py
+-rw-rw-rw-   0        0        0   106106 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/ndax.py
+-rw-rw-rw-   0        0        0    61638 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/novadax.py
+-rw-rw-rw-   0        0        0    37055 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/oceanex.py
+-rw-rw-rw-   0        0        0   177794 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/okcoin.py
+-rw-rw-rw-   0        0        0      434 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/okex.py
+-rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/okex5.py
+-rw-rw-rw-   0        0        0   264399 2023-06-15 05:48:33.000000 byquant-1.7.31/byquant/exchange/okx.py
+-rw-rw-rw-   0        0        0    22745 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/paymium.py
+-rw-rw-rw-   0        0        0   191805 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/phemex.py
+-rw-rw-rw-   0        0        0    88311 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/poloniex.py
+-rw-rw-rw-   0        0        0    75104 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/poloniexfutures.py
+-rw-rw-rw-   0        0        0    69774 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/probit.py
+-rw-rw-rw-   0        0        0    47325 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/ripio.py
+-rw-rw-rw-   0        0        0   117868 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/stex.py
+-rw-rw-rw-   0        0        0    42407 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/tidex.py
+-rw-rw-rw-   0        0        0    65452 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/timex.py
+-rw-rw-rw-   0        0        0   119250 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/tokocrypto.py
+-rw-rw-rw-   0        0        0    75531 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/upbit.py
+-rw-rw-rw-   0        0        0   103453 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/wavesexchange.py
+-rw-rw-rw-   0        0        0    35544 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/wazirx.py
+-rw-rw-rw-   0        0        0    92139 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/whitebit.py
+-rw-rw-rw-   0        0        0    94453 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/woo.py
+-rw-rw-rw-   0        0        0   196488 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/xt.py
+-rw-rw-rw-   0        0        0    51368 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/yobit.py
+-rw-rw-rw-   0        0        0    28777 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/zaif.py
+-rw-rw-rw-   0        0        0   183857 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/zb.py
+-rw-rw-rw-   0        0        0    74036 2023-05-14 16:20:52.000000 byquant-1.7.31/byquant/exchange/zonda.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:52:18.907459 byquant-1.7.31/byquant/indicator/
+-rw-rw-rw-   0        0        0     1017 2023-07-28 11:52:03.000000 byquant-1.7.31/byquant/indicator/__init__.py
+-rw-rw-rw-   0        0        0     1097 2023-07-31 02:51:15.000000 byquant-1.7.31/byquant/indicator/atr.py
+-rw-rw-rw-   0        0        0     1157 2023-07-31 02:50:20.000000 byquant-1.7.31/byquant/indicator/bbands.py
+-rw-rw-rw-   0        0        0     1099 2023-07-31 02:47:05.000000 byquant-1.7.31/byquant/indicator/cci.py
+-rw-rw-rw-   0        0        0     1078 2023-07-31 02:50:51.000000 byquant-1.7.31/byquant/indicator/dema.py
+-rw-rw-rw-   0        0        0     1074 2023-07-31 02:51:06.000000 byquant-1.7.31/byquant/indicator/ma.py
+-rw-rw-rw-   0        0        0     1161 2023-07-31 02:46:47.000000 byquant-1.7.31/byquant/indicator/macd.py
+-rw-rw-rw-   0        0        0     1105 2023-07-31 02:47:46.000000 byquant-1.7.31/byquant/indicator/rsi.py
+-rw-rw-rw-   0        0        0     1081 2023-07-31 02:43:20.000000 byquant-1.7.31/byquant/indicator/sma.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:52:18.959698 byquant-1.7.31/byquant/indicators/
+-rw-rw-rw-   0        0        0     1017 2023-07-28 11:52:03.000000 byquant-1.7.31/byquant/indicators/__init__.py
+-rw-rw-rw-   0        0        0     1253 2023-07-30 04:22:54.000000 byquant-1.7.31/byquant/indicators/atr.py
+-rw-rw-rw-   0        0        0     1253 2023-07-30 04:22:48.000000 byquant-1.7.31/byquant/indicators/cci.py
+-rw-rw-rw-   0        0        0     1254 2023-07-30 04:22:40.000000 byquant-1.7.31/byquant/indicators/macd.py
+-rw-rw-rw-   0        0        0     1254 2023-07-30 04:22:36.000000 byquant-1.7.31/byquant/indicators/rsi.py
+-rw-rw-rw-   0        0        0     1254 2023-07-30 04:24:59.000000 byquant-1.7.31/byquant/indicators/sma.py
+-rw-rw-rw-   0        0        0     1117 2023-07-30 04:29:44.000000 byquant-1.7.31/byquant/metastrategy.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:52:18.963692 byquant-1.7.31/byquant/strategy/
+-rw-rw-rw-   0        0        0      922 2023-07-30 04:49:12.000000 byquant-1.7.31/byquant/strategy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:52:18.974661 byquant-1.7.31/byquant/tool/
+-rw-rw-rw-   0        0        0        0 2023-06-27 01:25:40.000000 byquant-1.7.31/byquant/tool/__init__.py
+-rw-rw-rw-   0        0        0     3427 2023-02-15 05:30:28.000000 byquant-1.7.31/byquant/tool/tawPlus.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:52:18.192082 byquant-1.7.31/byquant.egg-info/
+-rw-rw-rw-   0        0        0     1451 2023-07-31 02:52:18.000000 byquant-1.7.31/byquant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4055 2023-07-31 02:52:18.000000 byquant-1.7.31/byquant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 02:52:18.000000 byquant-1.7.31/byquant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-07-31 02:52:18.000000 byquant-1.7.31/byquant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-31 02:52:18.000000 byquant-1.7.31/byquant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-15 09:08:59.000000 byquant-1.7.31/byquant.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      190 2023-07-31 02:51:51.000000 byquant-1.7.31/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-31 02:52:18.975697 byquant-1.7.31/setup.cfg
+-rw-rw-rw-   0        0        0     2880 2023-07-31 02:51:42.000000 byquant-1.7.31/setup.py
```

### Comparing `byquant-1.7.30/PKG-INFO` & `byquant-1.7.31/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byquant
-Version: 1.7.30
+Version: 1.7.31
 Summary: ByQuant.com is AI Quantitative Strategy Competition Training Community
 Home-page: https://byquant.com
 Author: Uakeey
 Author-email: uakee@outlook.com
 License: GPL
 Project-URL: Homepage, https://byquant.com
 Keywords: quant,strategy,algorithmic,algotrading
```

### Comparing `byquant-1.7.30/byquant/__init__.py` & `byquant-1.7.31/byquant/__init__.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/crypto/broker.py` & `byquant-1.7.31/byquant/crypto/broker.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/crypto/feed.py` & `byquant-1.7.31/byquant/crypto/feed.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/crypto/store.py` & `byquant-1.7.31/byquant/crypto/store.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/data/get.py` & `byquant-1.7.31/byquant/data/get.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/__init__.py` & `byquant-1.7.31/byquant/exchange/__init__.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/ace.py` & `byquant-1.7.31/byquant/exchange/ace.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/alpaca.py` & `byquant-1.7.31/byquant/exchange/alpaca.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/ascendex.py` & `byquant-1.7.31/byquant/exchange/ascendex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bequant.py` & `byquant-1.7.31/byquant/exchange/bequant.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bigone.py` & `byquant-1.7.31/byquant/exchange/bigone.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/binance.py` & `byquant-1.7.31/byquant/exchange/binance.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/binancecoinm.py` & `byquant-1.7.31/byquant/exchange/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/binanceus.py` & `byquant-1.7.31/byquant/exchange/binanceus.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/binanceusdm.py` & `byquant-1.7.31/byquant/exchange/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bit2c.py` & `byquant-1.7.31/byquant/exchange/bit2c.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bitbank.py` & `byquant-1.7.31/byquant/exchange/bitbank.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bitbns.py` & `byquant-1.7.31/byquant/exchange/bitbns.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bitfinex.py` & `byquant-1.7.31/byquant/exchange/bitfinex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bitfinex2.py` & `byquant-1.7.31/byquant/exchange/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bitflyer.py` & `byquant-1.7.31/byquant/exchange/bitflyer.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bitforex.py` & `byquant-1.7.31/byquant/exchange/bitforex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bitget.py` & `byquant-1.7.31/byquant/exchange/bitget.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bithumb.py` & `byquant-1.7.31/byquant/exchange/bithumb.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bitmart.py` & `byquant-1.7.31/byquant/exchange/bitmart.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bitmex.py` & `byquant-1.7.31/byquant/exchange/bitmex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bitopro.py` & `byquant-1.7.31/byquant/exchange/bitopro.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bitpanda.py` & `byquant-1.7.31/byquant/exchange/bitpanda.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bitrue.py` & `byquant-1.7.31/byquant/exchange/bitrue.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bitso.py` & `byquant-1.7.31/byquant/exchange/bitso.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bitstamp.py` & `byquant-1.7.31/byquant/exchange/bitstamp.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bitstamp1.py` & `byquant-1.7.31/byquant/exchange/bitstamp1.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bittrex.py` & `byquant-1.7.31/byquant/exchange/bittrex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bitvavo.py` & `byquant-1.7.31/byquant/exchange/bitvavo.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bkex.py` & `byquant-1.7.31/byquant/exchange/bkex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bl3p.py` & `byquant-1.7.31/byquant/exchange/bl3p.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/blockchaincom.py` & `byquant-1.7.31/byquant/exchange/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/btcalpha.py` & `byquant-1.7.31/byquant/exchange/btcalpha.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/btcbox.py` & `byquant-1.7.31/byquant/exchange/btcbox.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/btcex.py` & `byquant-1.7.31/byquant/exchange/btcex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/btcmarkets.py` & `byquant-1.7.31/byquant/exchange/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/btctradeua.py` & `byquant-1.7.31/byquant/exchange/btctradeua.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/btcturk.py` & `byquant-1.7.31/byquant/exchange/btcturk.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/buda.py` & `byquant-1.7.31/byquant/exchange/buda.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/bybit.py` & `byquant-1.7.31/byquant/exchange/bybit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/cex.py` & `byquant-1.7.31/byquant/exchange/cex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/coinbase.py` & `byquant-1.7.31/byquant/exchange/coinbase.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/coinbaseprime.py` & `byquant-1.7.31/byquant/exchange/coinbaseprime.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/coinbasepro.py` & `byquant-1.7.31/byquant/exchange/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/coincheck.py` & `byquant-1.7.31/byquant/exchange/coincheck.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/coinex.py` & `byquant-1.7.31/byquant/exchange/coinex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/coinfalcon.py` & `byquant-1.7.31/byquant/exchange/coinfalcon.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/coinmate.py` & `byquant-1.7.31/byquant/exchange/coinmate.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/coinone.py` & `byquant-1.7.31/byquant/exchange/coinone.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/coinsph.py` & `byquant-1.7.31/byquant/exchange/coinsph.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/coinspot.py` & `byquant-1.7.31/byquant/exchange/coinspot.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/cryptocom.py` & `byquant-1.7.31/byquant/exchange/cryptocom.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/currencycom.py` & `byquant-1.7.31/byquant/exchange/currencycom.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/delta.py` & `byquant-1.7.31/byquant/exchange/delta.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/deribit.py` & `byquant-1.7.31/byquant/exchange/deribit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/digifinex.py` & `byquant-1.7.31/byquant/exchange/digifinex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/exmo.py` & `byquant-1.7.31/byquant/exchange/exmo.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/flowbtc.py` & `byquant-1.7.31/byquant/exchange/flowbtc.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/fmfwio.py` & `byquant-1.7.31/byquant/exchange/fmfwio.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/gate.py` & `byquant-1.7.31/byquant/exchange/gate.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/gemini.py` & `byquant-1.7.31/byquant/exchange/gemini.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/hitbtc.py` & `byquant-1.7.31/byquant/exchange/hitbtc.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/hitbtc3.py` & `byquant-1.7.31/byquant/exchange/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/hollaex.py` & `byquant-1.7.31/byquant/exchange/hollaex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/huobi.py` & `byquant-1.7.31/byquant/exchange/huobi.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/huobijp.py` & `byquant-1.7.31/byquant/exchange/huobijp.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/huobipro.py` & `byquant-1.7.31/byquant/exchange/huobipro.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/idex.py` & `byquant-1.7.31/byquant/exchange/idex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/independentreserve.py` & `byquant-1.7.31/byquant/exchange/independentreserve.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/indodax.py` & `byquant-1.7.31/byquant/exchange/indodax.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/itbit.py` & `byquant-1.7.31/byquant/exchange/itbit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/kraken.py` & `byquant-1.7.31/byquant/exchange/kraken.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/krakenfutures.py` & `byquant-1.7.31/byquant/exchange/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/kucoin.py` & `byquant-1.7.31/byquant/exchange/kucoin.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/kucoinfutures.py` & `byquant-1.7.31/byquant/exchange/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/kuna.py` & `byquant-1.7.31/byquant/exchange/kuna.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/latoken.py` & `byquant-1.7.31/byquant/exchange/latoken.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/lbank.py` & `byquant-1.7.31/byquant/exchange/lbank.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/lbank2.py` & `byquant-1.7.31/byquant/exchange/lbank2.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/luno.py` & `byquant-1.7.31/byquant/exchange/luno.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/lykke.py` & `byquant-1.7.31/byquant/exchange/lykke.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/mercado.py` & `byquant-1.7.31/byquant/exchange/mercado.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/mexc.py` & `byquant-1.7.31/byquant/exchange/mexc.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/ndax.py` & `byquant-1.7.31/byquant/exchange/ndax.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/novadax.py` & `byquant-1.7.31/byquant/exchange/novadax.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/oceanex.py` & `byquant-1.7.31/byquant/exchange/oceanex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/okcoin.py` & `byquant-1.7.31/byquant/exchange/okcoin.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/okx.py` & `byquant-1.7.31/byquant/exchange/okx.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/paymium.py` & `byquant-1.7.31/byquant/exchange/paymium.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/phemex.py` & `byquant-1.7.31/byquant/exchange/phemex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/poloniex.py` & `byquant-1.7.31/byquant/exchange/poloniex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/poloniexfutures.py` & `byquant-1.7.31/byquant/exchange/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/probit.py` & `byquant-1.7.31/byquant/exchange/probit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/ripio.py` & `byquant-1.7.31/byquant/exchange/ripio.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/stex.py` & `byquant-1.7.31/byquant/exchange/stex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/tidex.py` & `byquant-1.7.31/byquant/exchange/tidex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/timex.py` & `byquant-1.7.31/byquant/exchange/timex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/tokocrypto.py` & `byquant-1.7.31/byquant/exchange/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/upbit.py` & `byquant-1.7.31/byquant/exchange/upbit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/wavesexchange.py` & `byquant-1.7.31/byquant/exchange/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/wazirx.py` & `byquant-1.7.31/byquant/exchange/wazirx.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/whitebit.py` & `byquant-1.7.31/byquant/exchange/whitebit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/woo.py` & `byquant-1.7.31/byquant/exchange/woo.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/xt.py` & `byquant-1.7.31/byquant/exchange/xt.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/yobit.py` & `byquant-1.7.31/byquant/exchange/yobit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/zaif.py` & `byquant-1.7.31/byquant/exchange/zaif.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/zb.py` & `byquant-1.7.31/byquant/exchange/zb.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/exchange/zonda.py` & `byquant-1.7.31/byquant/exchange/zonda.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/indicator/__init__.py` & `byquant-1.7.31/byquant/indicator/__init__.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/indicator/atr.py` & `byquant-1.7.31/byquant/indicators/cci.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,23 +15,18 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 ###############################################################################
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-import talib
+from __future__ import (absolute_import, division, print_function,unicode_literals)
+import backtrader as bt
 
-class ATR():
-    def __init__(self, data, period):
-        self.data = data
-        self.period = period
-        self._result = self._bydo()
-
-    def _bydo(self):
-        return talib.ATR(self.data.high, self.data.low, self.data.close, timeperiod=self.period)
-    
-    def __str__(self):
-        return str(self._result)
+class CCI(bt.Indicator):
+    lines = ('_bydo',)
+    params = (('period', 14),)
+    def __init__(self):
+        self._bydo = bt.indicators.CCI(self.data, period=self.p.period)
 
+    def next(self):
+        self.lines._bydo[0] = self._bydo[0]
```

### Comparing `byquant-1.7.30/byquant/indicator/bbands.py` & `byquant-1.7.31/byquant/indicators/atr.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,23 +15,18 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 ###############################################################################
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-import talib
+from __future__ import (absolute_import, division, print_function,unicode_literals)
+import backtrader as bt
 
-class BBANDS():
-    def __init__(self, data, timeperiod):
-        self.data = data
-        self.timeperiod = timeperiod
-        self.result = self._bbands()
+class ATR(bt.Indicator):
+    lines = ('_bydo',)
+    params = (('period', 14),)
+    def __init__(self):
+        self._bydo = bt.indicators.ATR(self.data, period=self.p.period)
 
-    def _bbands(self):
-        upper, middle, lower = talib.BBANDS(self.data.close, timeperiod=self.timeperiod,matype = talib.MA_Type.EMA)
-        return upper, middle, lower
-        
-    def __str__(self):
-        return str(self.result)
+    def next(self):
+        self.lines._bydo[0] = self._bydo[0]
```

### Comparing `byquant-1.7.30/byquant/indicator/cci.py` & `byquant-1.7.31/byquant/indicators/macd.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,23 +15,19 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 ###############################################################################
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-import talib
+from __future__ import (absolute_import, division, print_function,unicode_literals)
 
-class CCI():
-    def __init__(self, data, period):
-        self.data = data
-        self.period = period
-        self._result = self._bydo()
+import backtrader as bt
 
-    def _bydo(self):
-        return talib.CCI(self.data.high, self.data.low, self.data.close, timeperiod=self.period)
-    
-    def __str__(self):
-        return str(self._result)
+class RSI(bt.Indicator):
+    lines = ('_bydo',)
+    params = (('period', 14),)
+    def __init__(self):
+        self._bydo = bt.indicators.RSI(self.data, period=self.p.period)
 
+    def next(self):
+        self.lines._bydo[0] = self._bydo[0]
```

### Comparing `byquant-1.7.30/byquant/indicator/dema.py` & `byquant-1.7.31/byquant/indicators/rsi.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,22 +15,19 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 ###############################################################################
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-import talib
+from __future__ import (absolute_import, division, print_function,unicode_literals)
 
-class DEMA():
-    def __init__(self, data, timeperiod):
-        self.data = data
-        self.timeperiod = timeperiod
-        self.result = self._dema()
+import backtrader as bt
 
-    def _dema(self):
-        return talib.DEMA(self.data.close, timeperiod=self.timeperiod)
-    
-    def __str__(self):
-        return str(self.result)
+class RSI(bt.Indicator):
+    lines = ('_bydo',)
+    params = (('period', 14),)
+    def __init__(self):
+        self._bydo = bt.indicators.RSI(self.data, period=self.p.period)
+
+    def next(self):
+        self.lines._bydo[0] = self._bydo[0]
```

### Comparing `byquant-1.7.30/byquant/indicator/ma.py` & `byquant-1.7.31/byquant/indicators/sma.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,22 +15,19 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 ###############################################################################
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
-import talib
+from __future__ import (absolute_import, division, print_function,unicode_literals)
 
-class MA():
-    def __init__(self, data, timeperiod):
-        self.data = data
-        self.timeperiod = timeperiod
-        self.result = self._ma()
+import backtrader as bt
 
-    def _ma(self):
-        return talib.MA(self.data.close, timeperiod=self.timeperiod)
-    
-    def __str__(self):
-        return str(self.result)
+class SMA(bt.Indicator):
+    lines = ('_bydo',)
+    params = (('period', 14),)
+    def __init__(self):
+        self._bydo = bt.indicators.SMA(self.data, period=self.p.period)
+
+    def next(self):
+        self.lines._bydo[0] = self._bydo[0]
```

### Comparing `byquant-1.7.30/byquant/indicator/macd.py` & `byquant-1.7.31/byquant/indicator/macd.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,24 +15,12 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 ###############################################################################
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
+from __future__ import (absolute_import, division, print_function,unicode_literals)
 import talib
 
-class MACD():
-    def __init__(self, data, fastperiod, slowperiod, signalperiod):
-        self.data = data
-        self.fastperiod = fastperiod
-        self.slowperiod = slowperiod
-        self.signalperiod = signalperiod
-        self._result = self._bydo()
-
-    def _bydo(self):
-        return talib.MACD(self.data.close, fastperiod=self.fastperiod, slowperiod=self.slowperiod, signalperiod=self.signalperiod)
-    
-    def __str__(self):
-        return str(self._result)
+def MACD(data, fastperiod,slowperiod,signalperiod):
+    return talib.MACD(data.close, fastperiod=fastperiod, slowperiod=slowperiod, signalperiod=signalperiod)
```

### Comparing `byquant-1.7.30/byquant/indicator/rsi.py` & `byquant-1.7.31/byquant/indicator/rsi.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,19 +19,9 @@
 #
 ###############################################################################
 
 from __future__ import (absolute_import, division, print_function,
                         unicode_literals)
 import talib
 
-class RSI():
-    def __init__(self, data, period):
-        self.data = data
-        self.period = period
-        self._result = self._bydo()
-
-    def _bydo(self):
-        return talib.RSI(self.data.close, timeperiod=self.period)
-    
-    def __str__(self):
-        return str(self._result)
-
+def RSI(data, period):
+    return talib.RSI(data.close, timeperiod = period)
```

### Comparing `byquant-1.7.30/byquant/indicator/sma.py` & `byquant-1.7.31/byquant/indicator/sma.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,22 +15,16 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 ###############################################################################
 
-from __future__ import (absolute_import, division, print_function,
-                        unicode_literals)
+from __future__ import (absolute_import, division, print_function,unicode_literals)
 import talib
 
-class SMA():
-    def __init__(self, data, period):
-        self.data = data
-        self.period = period
-        self._result = self._bydo()
+def SMA(data,period):
+    return talib.SMA(data.close, timeperiod=period)
+
+
 
-    def _bydo(self):
-        return talib.SMA(self.data.close, timeperiod=self.period)
 
-    def __str__(self):
-        return str(self._result)
```

### Comparing `byquant-1.7.30/byquant/indicators/__init__.py` & `byquant-1.7.31/byquant/indicators/__init__.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/indicators/atr.py` & `byquant-1.7.31/byquant/indicator/ma.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,17 +16,11 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 ###############################################################################
 
 from __future__ import (absolute_import, division, print_function,unicode_literals)
-import backtrader as bt
+import talib
 
-class ATR(bt.Indicator):
-    lines = ('_bydo',)
-    params = (('period', 14),)
-    def __init__(self):
-        self._bydo = bt.indicators.ATR(self.data, period=self.p.period)
-
-    def next(self):
-        self.lines._bydo[0] = self._bydo[0]
+def MA(data,period):
+    return talib.MA(data.close, timeperiod=period)
```

### Comparing `byquant-1.7.30/byquant/indicators/cci.py` & `byquant-1.7.31/byquant/indicator/bbands.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,17 +16,12 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 ###############################################################################
 
 from __future__ import (absolute_import, division, print_function,unicode_literals)
-import backtrader as bt
+import talib
 
-class CCI(bt.Indicator):
-    lines = ('_bydo',)
-    params = (('period', 14),)
-    def __init__(self):
-        self._bydo = bt.indicators.CCI(self.data, period=self.p.period)
-
-    def next(self):
-        self.lines._bydo[0] = self._bydo[0]
+def BBANDS(data,period):
+    upper, middle, lower = talib.BBANDS(data.close, timeperiod=period,matype = talib.MA_Type.EMA)
+    return upper, middle, lower
```

### Comparing `byquant-1.7.30/byquant/indicators/macd.py` & `byquant-1.7.31/byquant/metastrategy.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,26 @@
-#!/usr/bin/env python
-# -*- coding: utf-8; py-indent-offset:4 -*-
-###############################################################################
-#
-# Copyright (C) 2022-2023 ByQuant.com
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-###############################################################################
-
-from __future__ import (absolute_import, division, print_function,unicode_literals)
-
-import backtrader as bt
-
-class RSI(bt.Indicator):
-    lines = ('_bydo',)
-    params = (('period', 14),)
-    def __init__(self):
-        self._bydo = bt.indicators.RSI(self.data, period=self.p.period)
-
-    def next(self):
-        self.lines._bydo[0] = self._bydo[0]
+#!/usr/bin/env python
+# -*- coding: utf-8; py-indent-offset:4 -*-
+###############################################################################
+#
+# Copyright (C) 2022-2023 ByQuant.com
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+#
+###############################################################################
+
+from __future__ import (absolute_import, division, print_function,unicode_literals)
+import backtrader as bt
+class Strategy(bt.Strategy):
+    def __init__(self):
+        super().__init__()
```

### Comparing `byquant-1.7.30/byquant/indicators/rsi.py` & `byquant-1.7.31/byquant/indicator/cci.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,18 +16,12 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 ###############################################################################
 
 from __future__ import (absolute_import, division, print_function,unicode_literals)
+import talib
 
-import backtrader as bt
+def CCI(data,period):
+    return talib.CCI(data.high, data.low, data.close, timeperiod=period)
 
-class RSI(bt.Indicator):
-    lines = ('_bydo',)
-    params = (('period', 14),)
-    def __init__(self):
-        self._bydo = bt.indicators.RSI(self.data, period=self.p.period)
-
-    def next(self):
-        self.lines._bydo[0] = self._bydo[0]
```

### Comparing `byquant-1.7.30/byquant/indicators/sma.py` & `byquant-1.7.31/byquant/indicator/dema.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,18 +16,11 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 ###############################################################################
 
 from __future__ import (absolute_import, division, print_function,unicode_literals)
+import talib
 
-import backtrader as bt
-
-class SMA(bt.Indicator):
-    lines = ('_bydo',)
-    params = (('period', 14),)
-    def __init__(self):
-        self._bydo = bt.indicators.SMA(self.data, period=self.p.period)
-
-    def next(self):
-        self.lines._bydo[0] = self._bydo[0]
+def DEMA(data,period):
+    return talib.DEMA(data.close, timeperiod=period)
```

### Comparing `byquant-1.7.30/byquant/metastrategy.py` & `byquant-1.7.31/byquant/indicator/atr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-#!/usr/bin/env python
-# -*- coding: utf-8; py-indent-offset:4 -*-
-###############################################################################
-#
-# Copyright (C) 2022-2023 ByQuant.com
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-###############################################################################
-
-from __future__ import (absolute_import, division, print_function,unicode_literals)
-import backtrader as bt
-class Strategy(bt.Strategy):
-    def __init__(self):
-        super().__init__()
+#!/usr/bin/env python
+# -*- coding: utf-8; py-indent-offset:4 -*-
+###############################################################################
+#
+# Copyright (C) 2022-2023 ByQuant.com
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+#
+###############################################################################
+
+from __future__ import (absolute_import, division, print_function,unicode_literals)
+import talib
+
+def ATR(data,period):
+    return talib.ATR(data.high, data.low, data.close, timeperiod=period)
```

### Comparing `byquant-1.7.30/byquant/strategy/__init__.py` & `byquant-1.7.31/byquant/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant/tool/tawPlus.py` & `byquant-1.7.31/byquant/tool/tawPlus.py`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/byquant.egg-info/PKG-INFO` & `byquant-1.7.31/byquant.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byquant
-Version: 1.7.30
+Version: 1.7.31
 Summary: ByQuant.com is AI Quantitative Strategy Competition Training Community
 Home-page: https://byquant.com
 Author: Uakeey
 Author-email: uakee@outlook.com
 License: GPL
 Project-URL: Homepage, https://byquant.com
 Keywords: quant,strategy,algorithmic,algotrading
```

### Comparing `byquant-1.7.30/byquant.egg-info/SOURCES.txt` & `byquant-1.7.31/byquant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `byquant-1.7.30/setup.py` & `byquant-1.7.31/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 here = path.abspath(path.dirname(__file__))
 root = path.dirname(here)
 
 readme = path.join(here, 'README.md')
 package = {
   "name": "byquant",
-  "version": "1.7.30",
+  "version": "1.7.31",
   "description": "ByQuant.com is AI Quantitative Strategy Competition Training Community",
   "type": "module",
   "readme": "README.md",
   "package_json": "package.json",
   "author": {
     "name": "Uakeey",
     "email": "uakee@outlook.com",
```

