# Comparing `tmp/defichainTest-0.0.1b0.tar.gz` & `tmp/defichainTest-0.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defichainTest-0.0.1b0.tar", last modified: Tue Jun 20 19:17:09 2023, max compression
+gzip compressed data, was "defichainTest-0.0.1b1.tar", last modified: Mon Jul 31 00:00:39 2023, max compression
```

## Comparing `defichainTest-0.0.1b0.tar` & `defichainTest-0.0.1b1.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.283062 defichainTest-0.0.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-06-20 19:17:09.279062 defichainTest-0.0.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.259062 defichainTest-0.0.1b0/defichain/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.259062 defichainTest-0.0.1b0/defichain/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.259062 defichainTest-0.0.1b0/defichain/exceptions/hdwallet/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/hdwallet/DerivationError.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/hdwallet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.259062 defichainTest-0.0.1b0/defichain/exceptions/http/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/http/BadMethod.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/http/BadRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/http/Forbidden.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/http/HTTPStatusCode.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/http/InternalServerError.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/http/NotFound.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/http/RPCErrorCode.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/http/ServiceUnavailable.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/http/Unauthorized.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/http/UnprocessableEntity.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/http/WrongParmeters.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.263062 defichainTest-0.0.1b0/defichain/exceptions/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/transactions/addresserror.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/transactions/defitxerror.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/transactions/deserializeerror.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/transactions/inputerror.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/transactions/keyerror.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/transactions/notsupported.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/transactions/rawtransactionerror.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/transactions/tokenerror.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/transactions/txbuildererror.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/exceptions/transactions/verifyerror.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.263062 defichainTest-0.0.1b0/defichain/hdwallet/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/hdwallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/hdwallet/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/hdwallet/derivations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/hdwallet/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    55798 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/hdwallet/wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.263062 defichainTest-0.0.1b0/defichain/libs/
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/libs/base58.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/libs/bech32.py
--rw-r--r--   0 runner    (1001) docker     (123)    14136 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/libs/ecc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/libs/ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.263062 defichainTest-0.0.1b0/defichain/mnemonic/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/mnemonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/mnemonic/mnemonic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.263062 defichainTest-0.0.1b0/defichain/mnemonic/wordlist/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/mnemonic/wordlist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/mnemonic/wordlist/chinese_simplified.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/mnemonic/wordlist/chinese_traditional.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/mnemonic/wordlist/english.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16776 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/mnemonic/wordlist/french.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16033 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/mnemonic/wordlist/italian.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26423 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/mnemonic/wordlist/japanese.txt
--rw-r--r--   0 runner    (1001) docker     (123)    37832 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/mnemonic/wordlist/korean.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13996 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/mnemonic/wordlist/spanish.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.263062 defichainTest-0.0.1b0/defichain/networks/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/networks/networks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.267062 defichainTest-0.0.1b0/defichain/node/
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/RPCErrorHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.267062 defichainTest-0.0.1b0/defichain/node/modules/
--rw-r--r--   0 runner    (1001) docker     (123)    21262 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/modules/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)    53564 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/modules/blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/modules/control.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/modules/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    14857 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/modules/loan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/modules/masternodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/modules/mining.py
--rw-r--r--   0 runner    (1001) docker     (123)    16833 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/modules/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/modules/oracles.py
--rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/modules/poolpair.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/modules/proposals.py
--rw-r--r--   0 runner    (1001) docker     (123)    40311 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/modules/rawtransactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/modules/spv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/modules/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    10291 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/modules/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/modules/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    15447 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/modules/vault.py
--rw-r--r--   0 runner    (1001) docker     (123)    86413 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/modules/wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/modules/zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/node/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.267062 defichainTest-0.0.1b0/defichain/ocean/
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/ocean/OceanErrorHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/ocean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/ocean/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.271062 defichainTest-0.0.1b0/defichain/ocean/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/ocean/modules/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/ocean/modules/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/ocean/modules/fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/ocean/modules/loan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/ocean/modules/masternodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/ocean/modules/oracles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/ocean/modules/poolpairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/ocean/modules/prices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/ocean/modules/rawTx.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/ocean/modules/rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/ocean/modules/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/ocean/modules/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/ocean/modules/transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/ocean/ocean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.271062 defichainTest-0.0.1b0/defichain/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.271062 defichainTest-0.0.1b0/defichain/transactions/address/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/address/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/address/base58address.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/address/baseaddress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/address/bech32address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/address/p2pkh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/address/p2sh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/address/p2wpkh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/address/script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.271062 defichainTest-0.0.1b0/defichain/transactions/builder/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/builder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.275062 defichainTest-0.0.1b0/defichain/transactions/builder/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/builder/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/builder/modules/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/builder/modules/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/builder/modules/utxo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/builder/rawtransactionbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/builder/txbuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.275062 defichainTest-0.0.1b0/defichain/transactions/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/constants/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/constants/defitx.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/constants/fees.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.275062 defichainTest-0.0.1b0/defichain/transactions/constants/mainnet/
--rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/constants/mainnet/CUSTOM_tokens.json
--rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/constants/mainnet/LIQUIDITY_tokens.json
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/constants/mainnet/LOAN_tokens.json
--rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/constants/mainnet/STANDARD_tokens.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/constants/mainnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/constants/opcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/constants/rawtransactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.275062 defichainTest-0.0.1b0/defichain/transactions/constants/testnet/
--rw-r--r--   0 runner    (1001) docker     (123)    18208 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/constants/testnet/CUSTOM_tokens.json
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/constants/testnet/LIQUIDITY_tokens.json
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/constants/testnet/LOAN_tokens.json
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/constants/testnet/STANDARD_tokens.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/constants/testnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/constants/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.275062 defichainTest-0.0.1b0/defichain/transactions/defitx/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/defitx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/defitx/builddefitx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/defitx/defitx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.279062 defichainTest-0.0.1b0/defichain/transactions/defitx/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/defitx/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/defitx/modules/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/defitx/modules/basedefitx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/defitx/modules/baseinput.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/defitx/modules/governance.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/defitx/modules/loans.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/defitx/modules/masternode.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/defitx/modules/oracles.py
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/defitx/modules/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/defitx/modules/token.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/defitx/modules/vault.py
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.279062 defichainTest-0.0.1b0/defichain/transactions/rawtransactions/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/rawtransactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/rawtransactions/fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/rawtransactions/sign.py
--rw-r--r--   0 runner    (1001) docker     (123)    19717 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/rawtransactions/tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/rawtransactions/txbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    14476 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/rawtransactions/txinput.py
--rw-r--r--   0 runner    (1001) docker     (123)    11295 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/rawtransactions/txoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/rawtransactions/witness.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.279062 defichainTest-0.0.1b0/defichain/transactions/remotedata/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/remotedata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/remotedata/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/remotedata/ocean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/remotedata/remotedata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.279062 defichainTest-0.0.1b0/defichain/transactions/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/utils/calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/utils/token.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/defichain/transactions/utils/verify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:17:09.279062 defichainTest-0.0.1b0/defichainTest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-06-20 19:17:09.000000 defichainTest-0.0.1b0/defichainTest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-06-20 19:17:09.000000 defichainTest-0.0.1b0/defichainTest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 19:17:09.000000 defichainTest-0.0.1b0/defichainTest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-20 19:17:09.000000 defichainTest-0.0.1b0/defichainTest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 19:17:09.000000 defichainTest-0.0.1b0/defichainTest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 19:17:09.283062 defichainTest-0.0.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-20 19:17:01.000000 defichainTest-0.0.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.917054 defichainTest-0.0.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-07-31 00:00:39.917054 defichainTest-0.0.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.889053 defichainTest-0.0.1b1/defichain/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.889053 defichainTest-0.0.1b1/defichain/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.889053 defichainTest-0.0.1b1/defichain/exceptions/hdwallet/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/hdwallet/DerivationError.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/hdwallet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.893053 defichainTest-0.0.1b1/defichain/exceptions/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/http/BadMethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/http/BadRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/http/Forbidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/http/HTTPStatusCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/http/InternalServerError.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/http/NotFound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/http/RPCErrorCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/http/ServiceUnavailable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/http/Unauthorized.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/http/UnprocessableEntity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/http/WrongParmeters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.893053 defichainTest-0.0.1b1/defichain/exceptions/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/transactions/addresserror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/transactions/defitxerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/transactions/deserializeerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/transactions/inputerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/transactions/keyerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/transactions/notsupported.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/transactions/rawtransactionerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/transactions/tokenerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/transactions/txbuildererror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/exceptions/transactions/verifyerror.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.893053 defichainTest-0.0.1b1/defichain/hdwallet/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/hdwallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/hdwallet/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/hdwallet/derivations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/hdwallet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55798 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/hdwallet/wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.893053 defichainTest-0.0.1b1/defichain/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/libs/base58.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/libs/bech32.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14136 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/libs/ecc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/libs/ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.897053 defichainTest-0.0.1b1/defichain/mnemonic/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/mnemonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/mnemonic/mnemonic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.897053 defichainTest-0.0.1b1/defichain/mnemonic/wordlist/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/mnemonic/wordlist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/mnemonic/wordlist/chinese_simplified.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/mnemonic/wordlist/chinese_traditional.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/mnemonic/wordlist/english.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16776 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/mnemonic/wordlist/french.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16033 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/mnemonic/wordlist/italian.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26423 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/mnemonic/wordlist/japanese.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    37832 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/mnemonic/wordlist/korean.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13996 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/mnemonic/wordlist/spanish.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.897053 defichainTest-0.0.1b1/defichain/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/networks/networks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.897053 defichainTest-0.0.1b1/defichain/node/
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/RPCErrorHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.901054 defichainTest-0.0.1b1/defichain/node/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)    21262 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/modules/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53564 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/modules/blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/modules/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/modules/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14857 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/modules/loan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/modules/masternodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/modules/mining.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16833 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/modules/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/modules/oracles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/modules/poolpair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/modules/proposals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40311 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/modules/rawtransactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/modules/spv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/modules/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10291 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/modules/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/modules/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15447 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/modules/vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86413 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/modules/wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/modules/zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/node/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.901054 defichainTest-0.0.1b1/defichain/ocean/
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/ocean/OceanErrorHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/ocean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/ocean/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.905053 defichainTest-0.0.1b1/defichain/ocean/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/ocean/modules/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/ocean/modules/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/ocean/modules/fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/ocean/modules/loan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/ocean/modules/masternodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/ocean/modules/oracles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/ocean/modules/poolpairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/ocean/modules/prices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/ocean/modules/rawTx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/ocean/modules/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/ocean/modules/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/ocean/modules/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/ocean/modules/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/ocean/ocean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.905053 defichainTest-0.0.1b1/defichain/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.905053 defichainTest-0.0.1b1/defichain/transactions/address/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/address/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/address/base58address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/address/baseaddress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/address/bech32address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/address/p2pkh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/address/p2sh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/address/p2wpkh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/address/script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.905053 defichainTest-0.0.1b1/defichain/transactions/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/builder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.905053 defichainTest-0.0.1b1/defichain/transactions/builder/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/builder/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/builder/modules/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/builder/modules/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/builder/modules/utxo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/builder/rawtransactionbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/builder/txbuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.909054 defichainTest-0.0.1b1/defichain/transactions/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/constants/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/constants/defitx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/constants/fees.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.909054 defichainTest-0.0.1b1/defichain/transactions/constants/mainnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/constants/mainnet/CUSTOM_tokens.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/constants/mainnet/LIQUIDITY_tokens.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/constants/mainnet/LOAN_tokens.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/constants/mainnet/STANDARD_tokens.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/constants/mainnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/constants/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/constants/rawtransactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.909054 defichainTest-0.0.1b1/defichain/transactions/constants/testnet/
+-rw-r--r--   0 runner    (1001) docker     (123)    18208 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/constants/testnet/CUSTOM_tokens.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/constants/testnet/LIQUIDITY_tokens.json
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/constants/testnet/LOAN_tokens.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/constants/testnet/STANDARD_tokens.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/constants/testnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/constants/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.909054 defichainTest-0.0.1b1/defichain/transactions/defitx/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/defitx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/defitx/builddefitx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/defitx/defitx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.913054 defichainTest-0.0.1b1/defichain/transactions/defitx/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/defitx/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/defitx/modules/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/defitx/modules/basedefitx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/defitx/modules/baseinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/defitx/modules/governance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/defitx/modules/loans.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/defitx/modules/masternode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/defitx/modules/oracles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/defitx/modules/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/defitx/modules/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/defitx/modules/vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.913054 defichainTest-0.0.1b1/defichain/transactions/rawtransactions/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/rawtransactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/rawtransactions/fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/rawtransactions/sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19717 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/rawtransactions/tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/rawtransactions/txbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14476 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/rawtransactions/txinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11295 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/rawtransactions/txoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/rawtransactions/witness.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.913054 defichainTest-0.0.1b1/defichain/transactions/remotedata/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/remotedata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/remotedata/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/remotedata/ocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/remotedata/remotedata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.913054 defichainTest-0.0.1b1/defichain/transactions/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/utils/calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/utils/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/defichain/transactions/utils/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:00:39.917054 defichainTest-0.0.1b1/defichainTest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-07-31 00:00:39.000000 defichainTest-0.0.1b1/defichainTest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-07-31 00:00:39.000000 defichainTest-0.0.1b1/defichainTest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 00:00:39.000000 defichainTest-0.0.1b1/defichainTest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-31 00:00:39.000000 defichainTest-0.0.1b1/defichainTest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-31 00:00:39.000000 defichainTest-0.0.1b1/defichainTest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 00:00:39.917054 defichainTest-0.0.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-31 00:00:27.000000 defichainTest-0.0.1b1/setup.py
```

### Comparing `defichainTest-0.0.1b0/LICENSE` & `defichainTest-0.0.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/exceptions/http/HTTPStatusCode.py` & `defichainTest-0.0.1b1/defichain/exceptions/http/HTTPStatusCode.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/exceptions/http/RPCErrorCode.py` & `defichainTest-0.0.1b1/defichain/exceptions/http/RPCErrorCode.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/exceptions/http/__init__.py` & `defichainTest-0.0.1b1/defichain/exceptions/http/__init__.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/hdwallet/account.py` & `defichainTest-0.0.1b1/defichain/hdwallet/account.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/hdwallet/derivations.py` & `defichainTest-0.0.1b1/defichain/hdwallet/derivations.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/hdwallet/utils.py` & `defichainTest-0.0.1b1/defichain/hdwallet/utils.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/hdwallet/wallet.py` & `defichainTest-0.0.1b1/defichain/hdwallet/wallet.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/libs/base58.py` & `defichainTest-0.0.1b1/defichain/libs/base58.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/libs/bech32.py` & `defichainTest-0.0.1b1/defichain/libs/bech32.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/libs/ecc.py` & `defichainTest-0.0.1b1/defichain/libs/ecc.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/libs/ripemd160.py` & `defichainTest-0.0.1b1/defichain/libs/ripemd160.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/logger.py` & `defichainTest-0.0.1b1/defichain/logger.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/mnemonic/mnemonic.py` & `defichainTest-0.0.1b1/defichain/mnemonic/mnemonic.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/mnemonic/wordlist/chinese_simplified.txt` & `defichainTest-0.0.1b1/defichain/mnemonic/wordlist/chinese_simplified.txt`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/mnemonic/wordlist/chinese_traditional.txt` & `defichainTest-0.0.1b1/defichain/mnemonic/wordlist/chinese_traditional.txt`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/mnemonic/wordlist/english.txt` & `defichainTest-0.0.1b1/defichain/mnemonic/wordlist/english.txt`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/mnemonic/wordlist/french.txt` & `defichainTest-0.0.1b1/defichain/mnemonic/wordlist/french.txt`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/mnemonic/wordlist/italian.txt` & `defichainTest-0.0.1b1/defichain/mnemonic/wordlist/italian.txt`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/mnemonic/wordlist/japanese.txt` & `defichainTest-0.0.1b1/defichain/mnemonic/wordlist/japanese.txt`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/mnemonic/wordlist/korean.txt` & `defichainTest-0.0.1b1/defichain/mnemonic/wordlist/korean.txt`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/mnemonic/wordlist/spanish.txt` & `defichainTest-0.0.1b1/defichain/mnemonic/wordlist/spanish.txt`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/networks/networks.py` & `defichainTest-0.0.1b1/defichain/networks/networks.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/node/RPCErrorHandler.py` & `defichainTest-0.0.1b1/defichain/node/RPCErrorHandler.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/node/__init__.py` & `defichainTest-0.0.1b1/defichain/node/__init__.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/node/modules/accounts.py` & `defichainTest-0.0.1b1/defichain/node/modules/accounts.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/node/modules/blockchain.py` & `defichainTest-0.0.1b1/defichain/node/modules/blockchain.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/node/modules/control.py` & `defichainTest-0.0.1b1/defichain/node/modules/control.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/node/modules/generating.py` & `defichainTest-0.0.1b1/defichain/node/modules/generating.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/node/modules/loan.py` & `defichainTest-0.0.1b1/defichain/node/modules/loan.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/node/modules/masternodes.py` & `defichainTest-0.0.1b1/defichain/node/modules/masternodes.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/node/modules/mining.py` & `defichainTest-0.0.1b1/defichain/node/modules/mining.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/node/modules/network.py` & `defichainTest-0.0.1b1/defichain/node/modules/network.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/node/modules/oracles.py` & `defichainTest-0.0.1b1/defichain/node/modules/oracles.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/node/modules/poolpair.py` & `defichainTest-0.0.1b1/defichain/node/modules/poolpair.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/node/modules/proposals.py` & `defichainTest-0.0.1b1/defichain/node/modules/proposals.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/node/modules/rawtransactions.py` & `defichainTest-0.0.1b1/defichain/node/modules/rawtransactions.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/node/modules/stats.py` & `defichainTest-0.0.1b1/defichain/node/modules/stats.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/node/modules/tokens.py` & `defichainTest-0.0.1b1/defichain/node/modules/tokens.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/node/modules/util.py` & `defichainTest-0.0.1b1/defichain/node/modules/util.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/node/modules/vault.py` & `defichainTest-0.0.1b1/defichain/node/modules/vault.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/node/modules/wallet.py` & `defichainTest-0.0.1b1/defichain/node/modules/wallet.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/node/modules/zmq.py` & `defichainTest-0.0.1b1/defichain/node/modules/zmq.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/node/node.py` & `defichainTest-0.0.1b1/defichain/node/node.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/node/rpc.py` & `defichainTest-0.0.1b1/defichain/node/rpc.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/node/util.py` & `defichainTest-0.0.1b1/defichain/node/util.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/ocean/OceanErrorHandler.py` & `defichainTest-0.0.1b1/defichain/ocean/OceanErrorHandler.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/ocean/__init__.py` & `defichainTest-0.0.1b1/defichain/ocean/__init__.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/ocean/connection.py` & `defichainTest-0.0.1b1/defichain/ocean/connection.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/ocean/modules/address.py` & `defichainTest-0.0.1b1/defichain/ocean/modules/address.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/ocean/modules/blocks.py` & `defichainTest-0.0.1b1/defichain/ocean/modules/blocks.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/ocean/modules/fee.py` & `defichainTest-0.0.1b1/defichain/ocean/modules/fee.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/ocean/modules/loan.py` & `defichainTest-0.0.1b1/defichain/ocean/modules/loan.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/ocean/modules/masternodes.py` & `defichainTest-0.0.1b1/defichain/ocean/modules/masternodes.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/ocean/modules/oracles.py` & `defichainTest-0.0.1b1/defichain/ocean/modules/oracles.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/ocean/modules/poolpairs.py` & `defichainTest-0.0.1b1/defichain/ocean/modules/poolpairs.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/ocean/modules/prices.py` & `defichainTest-0.0.1b1/defichain/ocean/modules/prices.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/ocean/modules/rawTx.py` & `defichainTest-0.0.1b1/defichain/ocean/modules/rawTx.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/ocean/modules/rpc.py` & `defichainTest-0.0.1b1/defichain/ocean/modules/rpc.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/ocean/modules/stats.py` & `defichainTest-0.0.1b1/defichain/ocean/modules/stats.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/ocean/modules/tokens.py` & `defichainTest-0.0.1b1/defichain/ocean/modules/tokens.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/ocean/modules/transactions.py` & `defichainTest-0.0.1b1/defichain/ocean/modules/transactions.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/ocean/ocean.py` & `defichainTest-0.0.1b1/defichain/ocean/ocean.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/address/address.py` & `defichainTest-0.0.1b1/defichain/transactions/address/address.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/address/base58address.py` & `defichainTest-0.0.1b1/defichain/transactions/address/base58address.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/address/baseaddress.py` & `defichainTest-0.0.1b1/defichain/transactions/address/baseaddress.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/address/bech32address.py` & `defichainTest-0.0.1b1/defichain/transactions/address/bech32address.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/address/p2pkh.py` & `defichainTest-0.0.1b1/defichain/transactions/address/p2pkh.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/address/p2sh.py` & `defichainTest-0.0.1b1/defichain/transactions/address/p2sh.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/address/p2wpkh.py` & `defichainTest-0.0.1b1/defichain/transactions/address/p2wpkh.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/address/script.py` & `defichainTest-0.0.1b1/defichain/transactions/address/script.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/builder/modules/accounts.py` & `defichainTest-0.0.1b1/defichain/transactions/builder/modules/accounts.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/builder/modules/pool.py` & `defichainTest-0.0.1b1/defichain/transactions/builder/modules/pool.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/builder/modules/utxo.py` & `defichainTest-0.0.1b1/defichain/transactions/builder/modules/utxo.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/builder/rawtransactionbuilder.py` & `defichainTest-0.0.1b1/defichain/transactions/builder/rawtransactionbuilder.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/builder/txbuilder.py` & `defichainTest-0.0.1b1/defichain/transactions/builder/txbuilder.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/constants/defitx.py` & `defichainTest-0.0.1b1/defichain/transactions/constants/defitx.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/constants/mainnet/CUSTOM_tokens.json` & `defichainTest-0.0.1b1/defichain/transactions/constants/mainnet/CUSTOM_tokens.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9367088607594937%*

 * *Differences: {'insert': "[(74, OrderedDict([('id', '221'), ('symbol', 'BTC'), ('name', 'Its'), ('isDAT', "*

 * *           "False), ('isLPS', False), ('isLoanToken', False)])), (75, OrderedDict([('id', '222'), "*

 * *           "('symbol', 'ETH'), ('name', 'even'), ('isDAT', False), ('isLPS', False), "*

 * *           "('isLoanToken', False)])), (76, OrderedDict([('id', '223'), ('symbol', 'USDT'), "*

 * *           "('name', 'funnier'), ('isDAT', False), ('isLPS', False), ('isLoanToken', False)])), "*

 * *           "(77, OrderedDict([('id', '2 […]*

```diff
@@ -586,9 +586,49 @@
     {
         "id": "201",
         "isDAT": false,
         "isLPS": false,
         "isLoanToken": false,
         "name": "Decentralized USD",
         "symbol": "DUSD"
+    },
+    {
+        "id": "221",
+        "isDAT": false,
+        "isLPS": false,
+        "isLoanToken": false,
+        "name": "Its",
+        "symbol": "BTC"
+    },
+    {
+        "id": "222",
+        "isDAT": false,
+        "isLPS": false,
+        "isLoanToken": false,
+        "name": "even",
+        "symbol": "ETH"
+    },
+    {
+        "id": "223",
+        "isDAT": false,
+        "isLPS": false,
+        "isLoanToken": false,
+        "name": "funnier",
+        "symbol": "USDT"
+    },
+    {
+        "id": "224",
+        "isDAT": false,
+        "isLPS": false,
+        "isLoanToken": false,
+        "name": "the second",
+        "symbol": "USDC"
+    },
+    {
+        "id": "225",
+        "isDAT": false,
+        "isLPS": false,
+        "isLoanToken": false,
+        "name": "time",
+        "symbol": "EUROC"
     }
 ]
```

### Comparing `defichainTest-0.0.1b0/defichain/transactions/constants/mainnet/LIQUIDITY_tokens.json` & `defichainTest-0.0.1b1/defichain/transactions/constants/mainnet/LIQUIDITY_tokens.json`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/constants/mainnet/LOAN_tokens.json` & `defichainTest-0.0.1b1/defichain/transactions/constants/mainnet/LOAN_tokens.json`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/constants/mainnet/STANDARD_tokens.json` & `defichainTest-0.0.1b1/defichain/transactions/constants/mainnet/STANDARD_tokens.json`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/constants/opcodes.py` & `defichainTest-0.0.1b1/defichain/transactions/constants/opcodes.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/constants/testnet/CUSTOM_tokens.json` & `defichainTest-0.0.1b1/defichain/transactions/constants/testnet/CUSTOM_tokens.json`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/constants/testnet/LIQUIDITY_tokens.json` & `defichainTest-0.0.1b1/defichain/transactions/constants/testnet/LIQUIDITY_tokens.json`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/constants/testnet/LOAN_tokens.json` & `defichainTest-0.0.1b1/defichain/transactions/constants/testnet/LOAN_tokens.json`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/constants/testnet/STANDARD_tokens.json` & `defichainTest-0.0.1b1/defichain/transactions/constants/testnet/STANDARD_tokens.json`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/constants/tokens.py` & `defichainTest-0.0.1b1/defichain/transactions/constants/tokens.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/defitx/builddefitx.py` & `defichainTest-0.0.1b1/defichain/transactions/defitx/builddefitx.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/defitx/defitx.py` & `defichainTest-0.0.1b1/defichain/transactions/defitx/defitx.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/defitx/modules/accounts.py` & `defichainTest-0.0.1b1/defichain/transactions/defitx/modules/accounts.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/defitx/modules/basedefitx.py` & `defichainTest-0.0.1b1/defichain/transactions/defitx/modules/basedefitx.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/defitx/modules/baseinput.py` & `defichainTest-0.0.1b1/defichain/transactions/defitx/modules/baseinput.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/defitx/modules/pool.py` & `defichainTest-0.0.1b1/defichain/transactions/defitx/modules/pool.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/keys.py` & `defichainTest-0.0.1b1/defichain/transactions/keys.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/rawtransactions/fee.py` & `defichainTest-0.0.1b1/defichain/transactions/rawtransactions/fee.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/rawtransactions/sign.py` & `defichainTest-0.0.1b1/defichain/transactions/rawtransactions/sign.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/rawtransactions/tx.py` & `defichainTest-0.0.1b1/defichain/transactions/rawtransactions/tx.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/rawtransactions/txbase.py` & `defichainTest-0.0.1b1/defichain/transactions/rawtransactions/txbase.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/rawtransactions/txinput.py` & `defichainTest-0.0.1b1/defichain/transactions/rawtransactions/txinput.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/rawtransactions/txoutput.py` & `defichainTest-0.0.1b1/defichain/transactions/rawtransactions/txoutput.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/rawtransactions/witness.py` & `defichainTest-0.0.1b1/defichain/transactions/rawtransactions/witness.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/remotedata/node.py` & `defichainTest-0.0.1b1/defichain/transactions/remotedata/node.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/remotedata/ocean.py` & `defichainTest-0.0.1b1/defichain/transactions/remotedata/ocean.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/remotedata/remotedata.py` & `defichainTest-0.0.1b1/defichain/transactions/remotedata/remotedata.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/utils/calculate.py` & `defichainTest-0.0.1b1/defichain/transactions/utils/calculate.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/utils/converter.py` & `defichainTest-0.0.1b1/defichain/transactions/utils/converter.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/utils/token.py` & `defichainTest-0.0.1b1/defichain/transactions/utils/token.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichain/transactions/utils/verify.py` & `defichainTest-0.0.1b1/defichain/transactions/utils/verify.py`

 * *Files identical despite different names*

### Comparing `defichainTest-0.0.1b0/defichainTest.egg-info/SOURCES.txt` & `defichainTest-0.0.1b1/defichainTest.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE
 MANIFEST.in
-README.md
+README.rst
 pyproject.toml
 requirements.txt
 setup.py
 defichain/__init__.py
 defichain/logger.py
 defichain/exceptions/__init__.py
 defichain/exceptions/hdwallet/DerivationError.py
```

### Comparing `defichainTest-0.0.1b0/setup.py` & `defichainTest-0.0.1b1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 from os import path
 
-VERSION = '0.0.1b0'
+VERSION = '0.0.1b1'
 DESCRIPTION = 'Defichain Python Library'
 
 # Project URLs
 project_urls = {
     "Tracker": "https://github.com/eric-volz/DefichainPython",
     "Documentation": "https://docs.defichain-python.de"
 }
 
 this_directory = path.abspath(path.dirname(__file__))
-with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+with open(path.join(this_directory, 'README.rst'), encoding='utf-8') as f:
     LONG_DESCRIPTION = f.read()
 
 # requirements.txt
 with open("requirements.txt", "r") as _requirements:
     requirements: list = list(map(str.strip, _requirements.read().split("\n")))
 
 # Setting up
@@ -23,15 +23,14 @@
     name="defichainTest",
     version=VERSION,
     author="Intr0c",
     author_email="introc@volz.link",
     url="https://github.com/eric-volz/DefichainPython",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
-    long_description_content_type='text/markdown',
     packages=['defichain',
               'defichain.exceptions',
               'defichain.exceptions.http',
               'defichain.exceptions.hdwallet',
               'defichain.exceptions.transactions',
               'defichain.libs',
               'defichain.mnemonic',
```

