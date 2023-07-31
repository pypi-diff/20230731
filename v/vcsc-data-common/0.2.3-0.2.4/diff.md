# Comparing `tmp/vcsc_data_common-0.2.3.tar.gz` & `tmp/vcsc_data_common-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcsc_data_common-0.2.3.tar", last modified: Sun Jul 30 15:33:16 2023, max compression
+gzip compressed data, was "vcsc_data_common-0.2.4.tar", last modified: Mon Jul 31 08:17:42 2023, max compression
```

## Comparing `vcsc_data_common-0.2.3.tar` & `vcsc_data_common-0.2.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.120073 vcsc_data_common-0.2.3/
--rw-r--r--   0 pd         (501) staff       (20)      300 2023-07-30 15:33:16.120181 vcsc_data_common-0.2.3/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      143 2023-02-22 09:16:04.000000 vcsc_data_common-0.2.3/README.md
--rw-r--r--   0 pd         (501) staff       (20)      799 2023-03-23 03:54:32.000000 vcsc_data_common-0.2.3/pyproject.toml
--rw-r--r--   0 pd         (501) staff       (20)      339 2023-07-30 15:33:16.120691 vcsc_data_common-0.2.3/setup.cfg
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.113367 vcsc_data_common-0.2.3/vcsc_data_common/
--rw-r--r--   0 pd         (501) staff       (20)      108 2023-02-22 09:07:01.000000 vcsc_data_common-0.2.3/vcsc_data_common/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.115213 vcsc_data_common-0.2.3/vcsc_data_common/ai_framework/
--rw-r--r--   0 pd         (501) staff       (20)       48 2023-02-22 09:02:01.000000 vcsc_data_common-0.2.3/vcsc_data_common/ai_framework/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     5081 2023-06-08 06:24:22.000000 vcsc_data_common-0.2.3/vcsc_data_common/ai_framework/interval_fetching.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.115901 vcsc_data_common-0.2.3/vcsc_data_common/backtest/
--rw-r--r--   0 pd         (501) staff       (20)     2537 2023-05-12 03:24:29.000000 vcsc_data_common-0.2.3/vcsc_data_common/backtest/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.116228 vcsc_data_common-0.2.3/vcsc_data_common/fiin_data/
--rw-r--r--   0 pd         (501) staff       (20)     2228 2023-07-30 15:31:52.000000 vcsc_data_common-0.2.3/vcsc_data_common/fiin_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.116493 vcsc_data_common-0.2.3/vcsc_data_common/live_price_data/
--rw-r--r--   0 pd         (501) staff       (20)     2347 2023-07-30 15:32:22.000000 vcsc_data_common-0.2.3/vcsc_data_common/live_price_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.116769 vcsc_data_common-0.2.3/vcsc_data_common/offline_price_data/
--rw-r--r--   0 pd         (501) staff       (20)      886 2023-07-30 15:32:20.000000 vcsc_data_common-0.2.3/vcsc_data_common/offline_price_data/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.117149 vcsc_data_common-0.2.3/vcsc_data_common/oneday_portfolio/
--rw-r--r--   0 pd         (501) staff       (20)      516 2023-05-24 09:25:19.000000 vcsc_data_common-0.2.3/vcsc_data_common/oneday_portfolio/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.117575 vcsc_data_common-0.2.3/vcsc_data_common/order/
--rw-r--r--   0 pd         (501) staff       (20)     3875 2023-06-08 02:36:37.000000 vcsc_data_common-0.2.3/vcsc_data_common/order/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.118261 vcsc_data_common-0.2.3/vcsc_data_common/portfolio_info/
--rw-r--r--   0 pd         (501) staff       (20)     3868 2023-06-13 08:25:14.000000 vcsc_data_common-0.2.3/vcsc_data_common/portfolio_info/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.118755 vcsc_data_common-0.2.3/vcsc_data_common/proprietary_trading/
--rw-r--r--   0 pd         (501) staff       (20)      740 2023-07-10 09:38:54.000000 vcsc_data_common-0.2.3/vcsc_data_common/proprietary_trading/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.119086 vcsc_data_common-0.2.3/vcsc_data_common/signals/
--rw-r--r--   0 pd         (501) staff       (20)     1513 2023-06-01 10:35:44.000000 vcsc_data_common-0.2.3/vcsc_data_common/signals/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-30 15:33:16.114433 vcsc_data_common-0.2.3/vcsc_data_common.egg-info/
--rw-r--r--   0 pd         (501) staff       (20)      300 2023-07-30 15:33:16.000000 vcsc_data_common-0.2.3/vcsc_data_common.egg-info/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)      736 2023-07-30 15:33:16.000000 vcsc_data_common-0.2.3/vcsc_data_common.egg-info/SOURCES.txt
--rw-r--r--   0 pd         (501) staff       (20)        1 2023-07-30 15:33:16.000000 vcsc_data_common-0.2.3/vcsc_data_common.egg-info/dependency_links.txt
--rw-r--r--   0 pd         (501) staff       (20)      140 2023-07-30 15:33:16.000000 vcsc_data_common-0.2.3/vcsc_data_common.egg-info/requires.txt
--rw-r--r--   0 pd         (501) staff       (20)       17 2023-07-30 15:33:16.000000 vcsc_data_common-0.2.3/vcsc_data_common.egg-info/top_level.txt
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-31 08:17:42.952818 vcsc_data_common-0.2.4/
+-rw-r--r--   0 pd         (501) staff       (20)      300 2023-07-31 08:17:42.952894 vcsc_data_common-0.2.4/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      143 2023-02-22 09:16:04.000000 vcsc_data_common-0.2.4/README.md
+-rw-r--r--   0 pd         (501) staff       (20)      799 2023-03-23 03:54:32.000000 vcsc_data_common-0.2.4/pyproject.toml
+-rw-r--r--   0 pd         (501) staff       (20)      339 2023-07-31 08:17:42.953196 vcsc_data_common-0.2.4/setup.cfg
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-31 08:17:42.948588 vcsc_data_common-0.2.4/vcsc_data_common/
+-rw-r--r--   0 pd         (501) staff       (20)      108 2023-02-22 09:07:01.000000 vcsc_data_common-0.2.4/vcsc_data_common/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-31 08:17:42.949987 vcsc_data_common-0.2.4/vcsc_data_common/ai_framework/
+-rw-r--r--   0 pd         (501) staff       (20)       48 2023-02-22 09:02:01.000000 vcsc_data_common-0.2.4/vcsc_data_common/ai_framework/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     5081 2023-06-08 06:24:22.000000 vcsc_data_common-0.2.4/vcsc_data_common/ai_framework/interval_fetching.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-31 08:17:42.950279 vcsc_data_common-0.2.4/vcsc_data_common/backtest/
+-rw-r--r--   0 pd         (501) staff       (20)     2537 2023-05-12 03:24:29.000000 vcsc_data_common-0.2.4/vcsc_data_common/backtest/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-31 08:17:42.950599 vcsc_data_common-0.2.4/vcsc_data_common/fiin_data/
+-rw-r--r--   0 pd         (501) staff       (20)     2228 2023-07-30 15:31:52.000000 vcsc_data_common-0.2.4/vcsc_data_common/fiin_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-31 08:17:42.950864 vcsc_data_common-0.2.4/vcsc_data_common/live_price_data/
+-rw-r--r--   0 pd         (501) staff       (20)     2347 2023-07-30 15:32:22.000000 vcsc_data_common-0.2.4/vcsc_data_common/live_price_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-31 08:17:42.951229 vcsc_data_common-0.2.4/vcsc_data_common/offline_price_data/
+-rw-r--r--   0 pd         (501) staff       (20)      886 2023-07-30 15:32:20.000000 vcsc_data_common-0.2.4/vcsc_data_common/offline_price_data/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-31 08:17:42.951434 vcsc_data_common-0.2.4/vcsc_data_common/oneday_portfolio/
+-rw-r--r--   0 pd         (501) staff       (20)      516 2023-05-24 09:25:19.000000 vcsc_data_common-0.2.4/vcsc_data_common/oneday_portfolio/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-31 08:17:42.951712 vcsc_data_common-0.2.4/vcsc_data_common/order/
+-rw-r--r--   0 pd         (501) staff       (20)     3875 2023-06-08 02:36:37.000000 vcsc_data_common-0.2.4/vcsc_data_common/order/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-31 08:17:42.951984 vcsc_data_common-0.2.4/vcsc_data_common/portfolio_info/
+-rw-r--r--   0 pd         (501) staff       (20)     3717 2023-07-31 08:16:46.000000 vcsc_data_common-0.2.4/vcsc_data_common/portfolio_info/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-31 08:17:42.952314 vcsc_data_common-0.2.4/vcsc_data_common/proprietary_trading/
+-rw-r--r--   0 pd         (501) staff       (20)      740 2023-07-10 09:38:54.000000 vcsc_data_common-0.2.4/vcsc_data_common/proprietary_trading/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-31 08:17:42.952589 vcsc_data_common-0.2.4/vcsc_data_common/signals/
+-rw-r--r--   0 pd         (501) staff       (20)     1513 2023-06-01 10:35:44.000000 vcsc_data_common-0.2.4/vcsc_data_common/signals/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-31 08:17:42.949488 vcsc_data_common-0.2.4/vcsc_data_common.egg-info/
+-rw-r--r--   0 pd         (501) staff       (20)      300 2023-07-31 08:17:42.000000 vcsc_data_common-0.2.4/vcsc_data_common.egg-info/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)      736 2023-07-31 08:17:42.000000 vcsc_data_common-0.2.4/vcsc_data_common.egg-info/SOURCES.txt
+-rw-r--r--   0 pd         (501) staff       (20)        1 2023-07-31 08:17:42.000000 vcsc_data_common-0.2.4/vcsc_data_common.egg-info/dependency_links.txt
+-rw-r--r--   0 pd         (501) staff       (20)      140 2023-07-31 08:17:42.000000 vcsc_data_common-0.2.4/vcsc_data_common.egg-info/requires.txt
+-rw-r--r--   0 pd         (501) staff       (20)       17 2023-07-31 08:17:42.000000 vcsc_data_common-0.2.4/vcsc_data_common.egg-info/top_level.txt
```

### Comparing `vcsc_data_common-0.2.3/pyproject.toml` & `vcsc_data_common-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.3/vcsc_data_common/ai_framework/interval_fetching.py` & `vcsc_data_common-0.2.4/vcsc_data_common/ai_framework/interval_fetching.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.3/vcsc_data_common/backtest/__init__.py` & `vcsc_data_common-0.2.4/vcsc_data_common/backtest/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.3/vcsc_data_common/fiin_data/__init__.py` & `vcsc_data_common-0.2.4/vcsc_data_common/fiin_data/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.3/vcsc_data_common/live_price_data/__init__.py` & `vcsc_data_common-0.2.4/vcsc_data_common/live_price_data/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.3/vcsc_data_common/offline_price_data/__init__.py` & `vcsc_data_common-0.2.4/vcsc_data_common/offline_price_data/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.3/vcsc_data_common/oneday_portfolio/__init__.py` & `vcsc_data_common-0.2.4/vcsc_data_common/oneday_portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.3/vcsc_data_common/order/__init__.py` & `vcsc_data_common-0.2.4/vcsc_data_common/order/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.3/vcsc_data_common/portfolio_info/__init__.py` & `vcsc_data_common-0.2.4/vcsc_data_common/portfolio_info/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,29 +28,27 @@
                 "balance","initBalance", t1."cutoffDate", "forceSellAmount" , t1."portfolioType",t1."diffBalanceRemain"
                 from "portfolio" t1
                 left join "symbol_info" t2 on t1.symbol = t2.symbol
                 left join "portfolio_config" t4 on t1."portfolioConfigId" = t4.id
 				WHERE t4.status = 'RUNNING'
         """, con=self.paper_trading_db_connection)
 
-    def update_target_percent_portfolio(self, portfolio_data: dict, portfolio_model: int,signals:dict,trading_model:int,trading_date:str=None):
+    def update_target_percent_portfolio(self, portfolio_data: dict, portfolio_model: int,trading_date:str=None):
 
         url = f"{self.paper_trading_api_end_point}/portfolioRatio/updateNewRatio"
 
         payload_data = {
             "ratio": portfolio_data,
             "portfolioModel": portfolio_model,
             "tradingDate": trading_date,
-            "signals":signals,
-            'tradingModel':trading_model
+            
         } if trading_date != None else {
             "ratio": portfolio_data,
             "portfolioModel": portfolio_model,
-            "signals":signals,
-            'tradingModel':trading_model
+          
         }
 
         payload = json.dumps(payload_data)
         headers = {
             'Content-Type': 'application/json'
         }
```

### Comparing `vcsc_data_common-0.2.3/vcsc_data_common/proprietary_trading/__init__.py` & `vcsc_data_common-0.2.4/vcsc_data_common/proprietary_trading/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.3/vcsc_data_common/signals/__init__.py` & `vcsc_data_common-0.2.4/vcsc_data_common/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `vcsc_data_common-0.2.3/vcsc_data_common.egg-info/SOURCES.txt` & `vcsc_data_common-0.2.4/vcsc_data_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

