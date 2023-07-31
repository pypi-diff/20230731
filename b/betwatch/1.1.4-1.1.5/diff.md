# Comparing `tmp/betwatch-1.1.4.tar.gz` & `tmp/betwatch-1.1.5.tar.gz`

## Comparing `betwatch-1.1.4.tar` & `betwatch-1.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-1.1.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 betwatch-1.1.4/Makefile
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.1.4/.github/dependabot.yml
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 betwatch-1.1.4/.github/workflows/test.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/__about__.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/__init__.py
--rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/client.py
--rw-r--r--   0        0        0    28031 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/client_async.py
--rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/queries.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/types/__init__.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/types/bookmakers.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/types/exceptions.py
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/types/filters.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/types/markets.py
--rw-r--r--   0        0        0    12663 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/types/race.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.1.4/betwatch/types/updates.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 betwatch-1.1.4/examples/get_race_prices.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 betwatch-1.1.4/examples/get_race_prices_async.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 betwatch-1.1.4/examples/get_races.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 betwatch-1.1.4/examples/get_races_async.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 betwatch-1.1.4/examples/subscriptions.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 betwatch-1.1.4/examples/update_rated_prices.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.1.4/tests/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 betwatch-1.1.4/tests/test_check_last_updated.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 betwatch-1.1.4/tests/test_get_race.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 betwatch-1.1.4/tests/test_get_race_async.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 betwatch-1.1.4/tests/test_get_races.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 betwatch-1.1.4/tests/test_get_races_async.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 betwatch-1.1.4/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.1.4/LICENSE.txt
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.1.4/README.md
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 betwatch-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 betwatch-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-1.1.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 betwatch-1.1.5/Makefile
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.1.5/.github/dependabot.yml
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 betwatch-1.1.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-1.1.5/betwatch/__about__.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 betwatch-1.1.5/betwatch/__init__.py
+-rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 betwatch-1.1.5/betwatch/client.py
+-rw-r--r--   0        0        0    28031 2020-02-02 00:00:00.000000 betwatch-1.1.5/betwatch/client_async.py
+-rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 betwatch-1.1.5/betwatch/queries.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.1.5/betwatch/types/__init__.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 betwatch-1.1.5/betwatch/types/bookmakers.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 betwatch-1.1.5/betwatch/types/exceptions.py
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 betwatch-1.1.5/betwatch/types/filters.py
+-rw-r--r--   0        0        0     5022 2020-02-02 00:00:00.000000 betwatch-1.1.5/betwatch/types/markets.py
+-rw-r--r--   0        0        0    12673 2020-02-02 00:00:00.000000 betwatch-1.1.5/betwatch/types/race.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.1.5/betwatch/types/updates.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 betwatch-1.1.5/examples/get_race_prices.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 betwatch-1.1.5/examples/get_race_prices_async.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 betwatch-1.1.5/examples/get_races.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 betwatch-1.1.5/examples/get_races_async.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 betwatch-1.1.5/examples/subscriptions.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 betwatch-1.1.5/examples/update_rated_prices.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.1.5/tests/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 betwatch-1.1.5/tests/test_check_last_updated.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 betwatch-1.1.5/tests/test_get_race.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 betwatch-1.1.5/tests/test_get_race_async.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 betwatch-1.1.5/tests/test_get_races.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 betwatch-1.1.5/tests/test_get_races_async.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 betwatch-1.1.5/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.1.5/LICENSE.txt
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.1.5/README.md
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 betwatch-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 betwatch-1.1.5/PKG-INFO
```

### Comparing `betwatch-1.1.4/.github/workflows/test.yml` & `betwatch-1.1.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.4/betwatch/__init__.py` & `betwatch-1.1.5/betwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.4/betwatch/client.py` & `betwatch-1.1.5/betwatch/client.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.4/betwatch/client_async.py` & `betwatch-1.1.5/betwatch/client_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.4/betwatch/queries.py` & `betwatch-1.1.5/betwatch/queries.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.4/betwatch/types/bookmakers.py` & `betwatch-1.1.5/betwatch/types/bookmakers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 
 
-class Bookmaker(Enum):
+class Bookmaker(str, Enum):
     TAB = "Tab"
     SPORTSBET = "Sportsbet"
     POINTSBET = "Pointsbet"
     UNIBET = "Unibet"
     NEDS = "Neds"
     LADBROKES = "Ladbrokes"
     BOOKMAKER = "Bookmaker"
```

### Comparing `betwatch-1.1.4/betwatch/types/filters.py` & `betwatch-1.1.5/betwatch/types/filters.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.4/betwatch/types/markets.py` & `betwatch-1.1.5/betwatch/types/markets.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     def __str__(self) -> str:
         return self.__repr__()
 
     def __post_init__(self):
         self.last_updated = dateutil.parser.isoparse(self._last_updated)
 
 
-class MarketPriceType(Enum):
+class MarketPriceType(str, Enum):
     FIXED_WIN = "FIXED_WIN"
     FIXED_PLACE = "FIXED_PLACE"
 
 
 @dataclass
 class BookmakerMarket:
     id: str
@@ -126,15 +126,15 @@
 
     def __post_init__(self):
         self.last_updated = (
             dateutil.parser.isoparse(self._last_updated) if self._last_updated else None
         )
 
 
-class BetfairSide(Enum):
+class BetfairSide(str, Enum):
     BACK = "BACK"
     LAY = "LAY"
 
 
 @dataclass
 class BetfairMarket:
     id: str
```

### Comparing `betwatch-1.1.4/betwatch/types/race.py` & `betwatch-1.1.5/betwatch/types/race.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 class SubscriptionUpdate:
     race_id: str
     bookmaker_markets: List[BookmakerMarket] = field(default_factory=list)
     betfair_markets: List[BetfairMarket] = field(default_factory=list)
     race_update: Optional["RaceUpdate"] = None
 
 
-class MeetingType(Enum):
+class MeetingType(str, Enum):
     THOROUGHBRED = "Thoroughbred"
     GREYHOUND = "Greyhound"
     HARNESS = "Harness"
 
     def __str__(self) -> str:
         if self == MeetingType.THOROUGHBRED:
             return "R"
         if self == MeetingType.GREYHOUND:
             return "G"
         if self == MeetingType.HARNESS:
             return "H"
         return "Unknown"
 
 
-class RaceStatus(Enum):
+class RaceStatus(str, Enum):
     OPEN = "Open"
     CLOSED = "Closed"
     ABANDONED = "Abandoned"
     INTERIM = "Interim"
     PAYING = "Paying"
     RESULTED = "Resulted"
```

### Comparing `betwatch-1.1.4/examples/get_race_prices.py` & `betwatch-1.1.5/examples/get_race_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.4/examples/get_race_prices_async.py` & `betwatch-1.1.5/examples/get_race_prices_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.4/examples/get_races.py` & `betwatch-1.1.5/examples/get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.4/examples/get_races_async.py` & `betwatch-1.1.5/examples/get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.4/examples/subscriptions.py` & `betwatch-1.1.5/examples/subscriptions.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.4/examples/update_rated_prices.py` & `betwatch-1.1.5/examples/update_rated_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.4/tests/test_get_race.py` & `betwatch-1.1.5/tests/test_get_race.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.4/tests/test_get_race_async.py` & `betwatch-1.1.5/tests/test_get_race_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.4/tests/test_get_races.py` & `betwatch-1.1.5/tests/test_get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.4/tests/test_get_races_async.py` & `betwatch-1.1.5/tests/test_get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.4/.gitignore` & `betwatch-1.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.4/LICENSE.txt` & `betwatch-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.4/README.md` & `betwatch-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.4/pyproject.toml` & `betwatch-1.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `betwatch-1.1.4/PKG-INFO` & `betwatch-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betwatch
-Version: 1.1.4
+Version: 1.1.5
 Summary: A Python package for interacting with the Betwatch.com API
 Project-URL: Documentation, https://github.com/betwatch/betwatch-sdk-python#readme
 Project-URL: Issues, https://github.com/betwatch/betwatch-sdk-python/issues
 Project-URL: Source, https://github.com/betwatch/betwatch-sdk-python
 Project-URL: Betwatch.com, https://betwatch.com
 Author-email: Jamie Watts <jamie@betwatch.com>
 License-File: LICENSE.txt
```

