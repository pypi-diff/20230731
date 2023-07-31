# Comparing `tmp/betwatch-1.1.3.tar.gz` & `tmp/betwatch-1.1.4.tar.gz`

## Comparing `betwatch-1.1.3.tar` & `betwatch-1.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-1.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 betwatch-1.1.3/Makefile
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.1.3/.github/dependabot.yml
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 betwatch-1.1.3/.github/workflows/test.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-1.1.3/betwatch/__about__.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 betwatch-1.1.3/betwatch/__init__.py
--rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 betwatch-1.1.3/betwatch/client.py
--rw-r--r--   0        0        0    28031 2020-02-02 00:00:00.000000 betwatch-1.1.3/betwatch/client_async.py
--rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 betwatch-1.1.3/betwatch/queries.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.1.3/betwatch/types/__init__.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 betwatch-1.1.3/betwatch/types/bookmakers.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 betwatch-1.1.3/betwatch/types/exceptions.py
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 betwatch-1.1.3/betwatch/types/filters.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 betwatch-1.1.3/betwatch/types/markets.py
--rw-r--r--   0        0        0    12576 2020-02-02 00:00:00.000000 betwatch-1.1.3/betwatch/types/race.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.1.3/betwatch/types/updates.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 betwatch-1.1.3/examples/get_race_prices.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 betwatch-1.1.3/examples/get_race_prices_async.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 betwatch-1.1.3/examples/get_races.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 betwatch-1.1.3/examples/get_races_async.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 betwatch-1.1.3/examples/subscriptions.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 betwatch-1.1.3/examples/update_rated_prices.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.1.3/tests/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 betwatch-1.1.3/tests/test_check_last_updated.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 betwatch-1.1.3/tests/test_get_race.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 betwatch-1.1.3/tests/test_get_race_async.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 betwatch-1.1.3/tests/test_get_races.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 betwatch-1.1.3/tests/test_get_races_async.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 betwatch-1.1.3/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.1.3/LICENSE.txt
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.1.3/README.md
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 betwatch-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 betwatch-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-1.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 betwatch-1.1.4/Makefile
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.1.4/.github/dependabot.yml
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 betwatch-1.1.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/__about__.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/__init__.py
+-rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/client.py
+-rw-r--r--   0        0        0    28031 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/client_async.py
+-rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/queries.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/types/__init__.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/types/bookmakers.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/types/exceptions.py
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/types/filters.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/types/markets.py
+-rw-r--r--   0        0        0    12663 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/types/race.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/types/updates.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 betwatch-1.1.4/examples/get_race_prices.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 betwatch-1.1.4/examples/get_race_prices_async.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 betwatch-1.1.4/examples/get_races.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 betwatch-1.1.4/examples/get_races_async.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 betwatch-1.1.4/examples/subscriptions.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 betwatch-1.1.4/examples/update_rated_prices.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.1.4/tests/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 betwatch-1.1.4/tests/test_check_last_updated.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 betwatch-1.1.4/tests/test_get_race.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 betwatch-1.1.4/tests/test_get_race_async.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 betwatch-1.1.4/tests/test_get_races.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 betwatch-1.1.4/tests/test_get_races_async.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 betwatch-1.1.4/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.1.4/LICENSE.txt
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.1.4/README.md
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 betwatch-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 betwatch-1.1.4/PKG-INFO
```

### Comparing `betwatch-1.1.3/.github/workflows/test.yml` & `betwatch-1.1.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.3/betwatch/__init__.py` & `betwatch-1.1.4/betwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.3/betwatch/client.py` & `betwatch-1.1.4/betwatch/client.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.3/betwatch/client_async.py` & `betwatch-1.1.4/betwatch/client_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.3/betwatch/queries.py` & `betwatch-1.1.4/betwatch/queries.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.3/betwatch/types/bookmakers.py` & `betwatch-1.1.4/betwatch/types/bookmakers.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.3/betwatch/types/filters.py` & `betwatch-1.1.4/betwatch/types/filters.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.3/betwatch/types/markets.py` & `betwatch-1.1.4/betwatch/types/markets.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.3/betwatch/types/race.py` & `betwatch-1.1.4/betwatch/types/race.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,15 +362,18 @@
         for runner in self.runners:
             market = runner.get_highest_bookmaker_market(
                 market_type=market_type, bookmakers=bookmakers
             )
             if not market:
                 continue
             price = market.get_price(market_type)
-            if not price or not price.price:
+            if not price or not price.price or price.price <= 1.01:
+                continue
+
+            if runner.scratched_time:
                 continue
 
             if not best_runners or not best_prices:
                 best_runners.append(runner)
                 best_prices.append(price)
                 continue
```

### Comparing `betwatch-1.1.3/examples/get_race_prices.py` & `betwatch-1.1.4/examples/get_race_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.3/examples/get_race_prices_async.py` & `betwatch-1.1.4/examples/get_race_prices_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.3/examples/get_races.py` & `betwatch-1.1.4/examples/get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.3/examples/get_races_async.py` & `betwatch-1.1.4/examples/get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.3/examples/subscriptions.py` & `betwatch-1.1.4/examples/subscriptions.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.3/examples/update_rated_prices.py` & `betwatch-1.1.4/examples/update_rated_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.3/tests/test_get_race.py` & `betwatch-1.1.4/tests/test_get_race.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.3/tests/test_get_race_async.py` & `betwatch-1.1.4/tests/test_get_race_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.3/tests/test_get_races.py` & `betwatch-1.1.4/tests/test_get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.3/tests/test_get_races_async.py` & `betwatch-1.1.4/tests/test_get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.3/.gitignore` & `betwatch-1.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.3/LICENSE.txt` & `betwatch-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.3/README.md` & `betwatch-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.3/pyproject.toml` & `betwatch-1.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.3/PKG-INFO` & `betwatch-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betwatch
-Version: 1.1.3
+Version: 1.1.4
 Summary: A Python package for interacting with the Betwatch.com API
 Project-URL: Documentation, https://github.com/betwatch/betwatch-sdk-python#readme
 Project-URL: Issues, https://github.com/betwatch/betwatch-sdk-python/issues
 Project-URL: Source, https://github.com/betwatch/betwatch-sdk-python
 Project-URL: Betwatch.com, https://betwatch.com
 Author-email: Jamie Watts <jamie@betwatch.com>
 License-File: LICENSE.txt
```

