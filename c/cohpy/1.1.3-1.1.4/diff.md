# Comparing `tmp/cohpy-1.1.3.tar.gz` & `tmp/cohpy-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohpy-1.1.3.tar", max compression
+gzip compressed data, was "cohpy-1.1.4.tar", max compression
```

## Comparing `cohpy-1.1.3.tar` & `cohpy-1.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1072 2023-07-30 20:00:45.343585 cohpy-1.1.3/LICENSE
--rw-r--r--   0        0        0     4725 2023-07-30 20:00:45.343585 cohpy-1.1.3/README.md
--rw-r--r--   0        0        0      542 2023-07-30 20:00:45.343585 cohpy-1.1.3/cohpy/__init__.py
--rw-r--r--   0        0        0     3755 2023-07-30 20:00:45.343585 cohpy-1.1.3/cohpy/client.py
--rw-r--r--   0        0        0      112 2023-07-30 20:00:45.343585 cohpy-1.1.3/cohpy/constants.py
--rw-r--r--   0        0        0     5437 2023-07-30 20:00:45.343585 cohpy-1.1.3/cohpy/endpoint.py
--rw-r--r--   0        0        0     1453 2023-07-30 20:00:45.343585 cohpy-1.1.3/cohpy/exceptions.py
--rw-r--r--   0        0        0      638 2023-07-30 20:00:45.343585 cohpy-1.1.3/cohpy/leaderboards.py
--rw-r--r--   0        0        0        0 2023-07-30 20:00:45.343585 cohpy-1.1.3/cohpy/tests/__init__.py
--rw-r--r--   0        0        0      856 2023-07-30 20:00:45.343585 cohpy-1.1.3/cohpy/tests/test_all_leaderboards.py
--rw-r--r--   0        0        0     3468 2023-07-30 20:00:45.347585 cohpy-1.1.3/cohpy/tests/test_personal_stat.py
--rw-r--r--   0        0        0     3276 2023-07-30 20:00:45.347585 cohpy-1.1.3/cohpy/tests/test_player_match_history.py
--rw-r--r--   0        0        0     3076 2023-07-30 20:00:45.347585 cohpy-1.1.3/cohpy/tests/test_specific_leaderboard.py
--rw-r--r--   0        0        0      361 2023-07-30 20:00:45.347585 cohpy-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     5241 1970-01-01 00:00:00.000000 cohpy-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-31 15:16:53.049177 cohpy-1.1.4/LICENSE
+-rw-r--r--   0        0        0     4736 2023-07-31 15:16:53.049177 cohpy-1.1.4/README.md
+-rw-r--r--   0        0        0      542 2023-07-31 15:16:53.049177 cohpy-1.1.4/cohpy/__init__.py
+-rw-r--r--   0        0        0     3759 2023-07-31 15:16:53.049177 cohpy-1.1.4/cohpy/client.py
+-rw-r--r--   0        0        0      112 2023-07-31 15:16:53.049177 cohpy-1.1.4/cohpy/constants.py
+-rw-r--r--   0        0        0     5429 2023-07-31 15:16:53.049177 cohpy-1.1.4/cohpy/endpoint.py
+-rw-r--r--   0        0        0     1443 2023-07-31 15:16:53.049177 cohpy-1.1.4/cohpy/exceptions.py
+-rw-r--r--   0        0        0      638 2023-07-31 15:16:53.053177 cohpy-1.1.4/cohpy/leaderboards.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:16:53.053177 cohpy-1.1.4/cohpy/tests/__init__.py
+-rw-r--r--   0        0        0      856 2023-07-31 15:16:53.053177 cohpy-1.1.4/cohpy/tests/test_all_leaderboards.py
+-rw-r--r--   0        0        0     3468 2023-07-31 15:16:53.053177 cohpy-1.1.4/cohpy/tests/test_personal_stat.py
+-rw-r--r--   0        0        0     3276 2023-07-31 15:16:53.053177 cohpy-1.1.4/cohpy/tests/test_player_match_history.py
+-rw-r--r--   0        0        0     3076 2023-07-31 15:16:53.053177 cohpy-1.1.4/cohpy/tests/test_specific_leaderboard.py
+-rw-r--r--   0        0        0      361 2023-07-31 15:16:53.053177 cohpy-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5252 1970-01-01 00:00:00.000000 cohpy-1.1.4/PKG-INFO
```

### Comparing `cohpy-1.1.3/LICENSE` & `cohpy-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cohpy-1.1.3/README.md` & `cohpy-1.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 ````
 
 api_client.leaderboards():
 : Get all leaderboards available from the COH API
 
 - Parameters:
   - leaderboard_id (mandatory): Leaderboard identifier extracted from leaderboards() function. You can use raw ints like 2130329 or
-Code class that wraps more used leaderboards
+Code enum that wraps most used leaderboards
   - count (optional): **Default=200** How many players will be showed in the response. From 1 to 200.
   - sort_type (optional): **Default=ELO** Set the order of the leaderboard based on wins or elo. You can use ints like 0 (ELO) or 1 (WINS). Also you can use SortType wrapper
   - start (optional): **Default=1** Sets the position of the first player obtained from the request.
   - remove_server_status (optional): **Default=True** Remove from the response the server status (redundant).
 You can show it setting this param to **False**
 ````python
 import cohpy
@@ -90,15 +90,15 @@
 
 ````
 
 api_client.personal_stats():
 : Get all leaderboards available from the COH API
 
 - Parameters:
-  - profile_params (mandatory): Player id. Can be steam profile id, relic id or alias (Don't forget to set the mode). Can be a list of ints or strings. Steam queries must follow /steam/[0-9]+
+  - profile_params (mandatory): Player id. Can be steam profile id, relic id or alias (Don't forget to set the mode). It can be a list of ints or strings. Steam queries must follow /steam/[0-9]+ pattern.
   - mode (optional): **Default=relic** Set the query mode. Options are [relic, steam, alias].
   - remove_server_status (optional): **Default=True** Remove from the response the server status (redundant).
 You can show it setting this param to **False**
 ````python
 import cohpy
 
 api_client = cohpy.get_api_client()
```

#### html2text {}

```diff
@@ -12,16 +12,16 @@
 api_client = cohpy.get_api_client() ```` api_client.leaderboards(): : Get all
 leaderboards available from the COH API - Parameters: - remove_server_status
 (optional): **Default=True** Remove from the response the server status
 (redundant). You can show it setting this param to **False** ````python import
 cohpy api_client = cohpy.get_api_client() api_client.leaderboards() ````
 api_client.leaderboards(): : Get all leaderboards available from the COH API -
 Parameters: - leaderboard_id (mandatory): Leaderboard identifier extracted from
-leaderboards() function. You can use raw ints like 2130329 or Code class that
-wraps more used leaderboards - count (optional): **Default=200** How many
+leaderboards() function. You can use raw ints like 2130329 or Code enum that
+wraps most used leaderboards - count (optional): **Default=200** How many
 players will be showed in the response. From 1 to 200. - sort_type (optional):
 **Default=ELO** Set the order of the leaderboard based on wins or elo. You can
 use ints like 0 (ELO) or 1 (WINS). Also you can use SortType wrapper - start
 (optional): **Default=1** Sets the position of the first player obtained from
 the request. - remove_server_status (optional): **Default=True** Remove from
 the response the server status (redundant). You can show it setting this param
 to **False** ````python import cohpy api_client = cohpy.get_api_client()
@@ -36,26 +36,26 @@
 param to **False** ````python import cohpy api_client = cohpy.get_api_client()
 api_client.match_history(profile_params=[1, 2]) api_client.match_history
 (profile_params=1) api_client.match_history(profile_params='/steam/123456789',
 mode='steam') api_client.match_history(profile_params=['/steam/123456789', '/
 steam/123456789'], mode='steam') ```` api_client.personal_stats(): : Get all
 leaderboards available from the COH API - Parameters: - profile_params
 (mandatory): Player id. Can be steam profile id, relic id or alias (Don't
-forget to set the mode). Can be a list of ints or strings. Steam queries must
-follow /steam/[0-9]+ - mode (optional): **Default=relic** Set the query mode.
-Options are [relic, steam, alias]. - remove_server_status (optional):
-**Default=True** Remove from the response the server status (redundant). You
-can show it setting this param to **False** ````python import cohpy api_client
-= cohpy.get_api_client() api_client.personal_stats(profile_params=[1, 2])
-api_client.personal_stats(profile_params=1) api_client.personal_stats
-(profile_params='/steam/123456789', mode='steam') api_client.personal_stats
-(profile_params=['/steam/123456789', '/steam/123456789'], mode='steam')
-api_client.personal_stats(profile_params='yoursuperalias', mode='alias')
-api_client.personal_stats(profile_params=['yoursuperalias', 'awesomealias'],
-mode='alias') ```` # Examples First of all, you'll need an APIClient instance
-to retrieve the api data: ````python import cohpy api_client =
-cohpy.get_api_client() ```` Then you could use the API interface to retrieve
-the data you want: ````python import cohpy all_leaderboards =
-api_client.leaderboards() # Returns all leaderboards info
-american_3v3_leaderboard = api_client.leaderboard
+forget to set the mode). It can be a list of ints or strings. Steam queries
+must follow /steam/[0-9]+ pattern. - mode (optional): **Default=relic** Set the
+query mode. Options are [relic, steam, alias]. - remove_server_status
+(optional): **Default=True** Remove from the response the server status
+(redundant). You can show it setting this param to **False** ````python import
+cohpy api_client = cohpy.get_api_client() api_client.personal_stats
+(profile_params=[1, 2]) api_client.personal_stats(profile_params=1)
+api_client.personal_stats(profile_params='/steam/123456789', mode='steam')
+api_client.personal_stats(profile_params=['/steam/123456789', '/steam/
+123456789'], mode='steam') api_client.personal_stats
+(profile_params='yoursuperalias', mode='alias') api_client.personal_stats
+(profile_params=['yoursuperalias', 'awesomealias'], mode='alias') ```` #
+Examples First of all, you'll need an APIClient instance to retrieve the api
+data: ````python import cohpy api_client = cohpy.get_api_client() ```` Then you
+could use the API interface to retrieve the data you want: ````python import
+cohpy all_leaderboards = api_client.leaderboards() # Returns all leaderboards
+info american_3v3_leaderboard = api_client.leaderboard
 (leaderboard_id=cohpy.Codes.USF3v3) # Returns info from specific leaderboard
 ```` Note that ````leaderboard_id```` can be a int or a cohpy.Codes instance.
```

### Comparing `cohpy-1.1.3/cohpy/__init__.py` & `cohpy-1.1.4/cohpy/__init__.py`

 * *Files identical despite different names*

### Comparing `cohpy-1.1.3/cohpy/client.py` & `cohpy-1.1.4/cohpy/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,18 @@
         if remove_server_status:
             response.pop('result')
         return response
 
     def leaderboard(self, *, leaderboard_id, remove_server_status=True, count=200,
                     sort_type=SortType.ELO, start=1):
         """
-        Retrieve data about a specific leaderboard given her id.
+        Retrieve data about a specific leaderboard given its id.
 
         :param start: Position of the first player in the requests
-        :param sort_type: 1 == Sort by Wins, 0 == Sort by ELO. int or Type instance
+        :param sort_type: 1 == Sort by Wins, 0 == Sort by ELO. int or SortType instance
         :param count: How many players will be returned [1-200]
         :param leaderboard_id: int or cohpy.leaderboards.Code
         :param remove_server_status: Set to False if you want the server status response.
         :return: leaderboard info dict
         """
         if isinstance(leaderboard_id, Codes):
             leaderboard_id = leaderboard_id.value
```

### Comparing `cohpy-1.1.3/cohpy/endpoint.py` & `cohpy-1.1.4/cohpy/endpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,68 +106,68 @@
         """
         Validate that all steam profiles id are str and startswith steam/
 
         Regex explanation:
 
         - ^ is an anchor that specifies the beginning of the string.
         - This means that the string being matched must start with /steam/.
-        - [0-9] is a character set that matches any digit (0-9).
+        - d is a python shortcut for digits
         - (+) quantifier specifies that the digit character set must occur one or more times.
 
          Examples:
 
         - /steam/123
         - /steam/0
         - /steam/9876543210
         :return:
         """
         self.profile_params = self.profile_params.split() if type(self.profile_params) is str \
             else self.profile_params
-        pattern = re.compile(r'^/steam/[0-9]+')
+        pattern = re.compile(r'^/steam/\d+')
         if not all(type(param) is str and re.fullmatch(pattern, param)
                    for param in self.profile_params):
             raise BadSteamIdExpression()
 
     def _validate_relic_params(self):
         """
         Validate all relic's params are int
         :return:
         """
         self.profile_params = [self.profile_params] if type(self.profile_params) is not list else \
             self.profile_params
-        if not all(type(param) == int for param in self.profile_params):
+        if not all(isinstance(param, int) for param in self.profile_params):
             raise BadRelicIdExpression()
 
     def _validate_aliases_params(self):
         """
         Validate all aliases params are str
         :return:
         """
         self.profile_params = self.profile_params.split() if type(self.profile_params) is str \
             else self.profile_params
         if isinstance(self.profile_params, Iterable):
-            if not all(type(param) == str for param in self.profile_params):
+            if not all(isinstance(param, str) for param in self.profile_params):
                 raise BadAliasesExpression()
         else:
-            if type(self.profile_params) != str:
+            if not isinstance(self.profile_params, str):
                 raise BadAliasesExpression()
 
 
 @dataclass
 class AllLeaderboards(Endpoint):
     """
     Return all the available leaderboards
     """
     action: str = 'leaderboard/getAvailableLeaderboards/'
 
 
 @dataclass
 class Leaderboard(Endpoint):
     """
-    Return concrete data about a leaderboard
+    Return specific data about a leaderboard
     """
     action: str = 'leaderboard/getleaderboard2'
 
 
 @dataclass
 class MatchHistory(PlayersEndpoint):
     """
```

### Comparing `cohpy-1.1.3/cohpy/exceptions.py` & `cohpy-1.1.4/cohpy/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 class CoreException(Exception):
     def __init__(self, failure_msg):
         self.failure_msg = failure_msg
         super().__init__(self.failure_msg)
 
-    pass
-
 
 class LeaderBoardDoesNotExist(CoreException):
     def __init__(self, leaderboard_id):
         self.failure_msg = f'Leaderboard with id: {leaderboard_id} does not exists.'
         super().__init__(self.failure_msg)
```

### Comparing `cohpy-1.1.3/cohpy/leaderboards.py` & `cohpy-1.1.4/cohpy/leaderboards.py`

 * *Files identical despite different names*

### Comparing `cohpy-1.1.3/cohpy/tests/test_all_leaderboards.py` & `cohpy-1.1.4/cohpy/tests/test_all_leaderboards.py`

 * *Files identical despite different names*

### Comparing `cohpy-1.1.3/cohpy/tests/test_personal_stat.py` & `cohpy-1.1.4/cohpy/tests/test_personal_stat.py`

 * *Files identical despite different names*

### Comparing `cohpy-1.1.3/cohpy/tests/test_player_match_history.py` & `cohpy-1.1.4/cohpy/tests/test_player_match_history.py`

 * *Files identical despite different names*

### Comparing `cohpy-1.1.3/cohpy/tests/test_specific_leaderboard.py` & `cohpy-1.1.4/cohpy/tests/test_specific_leaderboard.py`

 * *Files identical despite different names*

### Comparing `cohpy-1.1.3/PKG-INFO` & `cohpy-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: cohpy
-Version: 1.1.3
+Version: 1.1.4
 Summary: 
 Author: Andres Garrido
 Author-email: andreslp0001@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: coverage (>=7.2.2,<8.0.0)
-Requires-Dist: flake8 (>=6.0.0,<7.0.0)
+Requires-Dist: coverage (>=7.2.7,<8.0.0)
+Requires-Dist: flake8 (>=6.1.0,<7.0.0)
 Requires-Dist: flake8-import-order (>=0.18.2,<0.19.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <h1 style="text-align: center">COHPY</h1>
 <div style="text-align: center">
 <i>An unofficial API Wrapper for Company Of Heroes API</i>
 
 </div>
@@ -68,15 +68,15 @@
 ````
 
 api_client.leaderboards():
 : Get all leaderboards available from the COH API
 
 - Parameters:
   - leaderboard_id (mandatory): Leaderboard identifier extracted from leaderboards() function. You can use raw ints like 2130329 or
-Code class that wraps more used leaderboards
+Code enum that wraps most used leaderboards
   - count (optional): **Default=200** How many players will be showed in the response. From 1 to 200.
   - sort_type (optional): **Default=ELO** Set the order of the leaderboard based on wins or elo. You can use ints like 0 (ELO) or 1 (WINS). Also you can use SortType wrapper
   - start (optional): **Default=1** Sets the position of the first player obtained from the request.
   - remove_server_status (optional): **Default=True** Remove from the response the server status (redundant).
 You can show it setting this param to **False**
 ````python
 import cohpy
@@ -106,15 +106,15 @@
 
 ````
 
 api_client.personal_stats():
 : Get all leaderboards available from the COH API
 
 - Parameters:
-  - profile_params (mandatory): Player id. Can be steam profile id, relic id or alias (Don't forget to set the mode). Can be a list of ints or strings. Steam queries must follow /steam/[0-9]+
+  - profile_params (mandatory): Player id. Can be steam profile id, relic id or alias (Don't forget to set the mode). It can be a list of ints or strings. Steam queries must follow /steam/[0-9]+ pattern.
   - mode (optional): **Default=relic** Set the query mode. Options are [relic, steam, alias].
   - remove_server_status (optional): **Default=True** Remove from the response the server status (redundant).
 You can show it setting this param to **False**
 ````python
 import cohpy
 
 api_client = cohpy.get_api_client()
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: cohpy Version: 1.1.3 Summary: Author: Andres
+Metadata-Version: 2.1 Name: cohpy Version: 1.1.4 Summary: Author: Andres
 Garrido Author-email: andreslp0001@gmail.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: coverage (>=7.2.2,<8.0.0) Requires-Dist: flake8 (>=6.0.0,<7.0.0)
+Requires-Dist: coverage (>=7.2.7,<8.0.0) Requires-Dist: flake8 (>=6.1.0,<7.0.0)
 Requires-Dist: flake8-import-order (>=0.18.2,<0.19.0) Requires-Dist: requests
-(>=2.28.2,<3.0.0) Description-Content-Type: text/markdown
+(>=2.31.0,<3.0.0) Description-Content-Type: text/markdown
 ****** COHPY ******
 An unofficial API Wrapper for Company Of Heroes API
 [![Lint and Tests](https://github.com/AndresGL01/cohpy/actions/workflows/
 ci.yml/badge.svg)](https://github.com/AndresGL01/cohpy/actions/workflows/
 ci.yml) [Stars_Badge] ### Tutorial - [How to install](#How-to-install) -
 [Functionalities](#Functionalities) - [Examples](#Examples) ## How to install
 ````shell pip install cohpy ```` Visit [Pypi](https://pypi.org/project/cohpy/
@@ -19,16 +19,16 @@
 api_client = cohpy.get_api_client() ```` api_client.leaderboards(): : Get all
 leaderboards available from the COH API - Parameters: - remove_server_status
 (optional): **Default=True** Remove from the response the server status
 (redundant). You can show it setting this param to **False** ````python import
 cohpy api_client = cohpy.get_api_client() api_client.leaderboards() ````
 api_client.leaderboards(): : Get all leaderboards available from the COH API -
 Parameters: - leaderboard_id (mandatory): Leaderboard identifier extracted from
-leaderboards() function. You can use raw ints like 2130329 or Code class that
-wraps more used leaderboards - count (optional): **Default=200** How many
+leaderboards() function. You can use raw ints like 2130329 or Code enum that
+wraps most used leaderboards - count (optional): **Default=200** How many
 players will be showed in the response. From 1 to 200. - sort_type (optional):
 **Default=ELO** Set the order of the leaderboard based on wins or elo. You can
 use ints like 0 (ELO) or 1 (WINS). Also you can use SortType wrapper - start
 (optional): **Default=1** Sets the position of the first player obtained from
 the request. - remove_server_status (optional): **Default=True** Remove from
 the response the server status (redundant). You can show it setting this param
 to **False** ````python import cohpy api_client = cohpy.get_api_client()
@@ -43,26 +43,26 @@
 param to **False** ````python import cohpy api_client = cohpy.get_api_client()
 api_client.match_history(profile_params=[1, 2]) api_client.match_history
 (profile_params=1) api_client.match_history(profile_params='/steam/123456789',
 mode='steam') api_client.match_history(profile_params=['/steam/123456789', '/
 steam/123456789'], mode='steam') ```` api_client.personal_stats(): : Get all
 leaderboards available from the COH API - Parameters: - profile_params
 (mandatory): Player id. Can be steam profile id, relic id or alias (Don't
-forget to set the mode). Can be a list of ints or strings. Steam queries must
-follow /steam/[0-9]+ - mode (optional): **Default=relic** Set the query mode.
-Options are [relic, steam, alias]. - remove_server_status (optional):
-**Default=True** Remove from the response the server status (redundant). You
-can show it setting this param to **False** ````python import cohpy api_client
-= cohpy.get_api_client() api_client.personal_stats(profile_params=[1, 2])
-api_client.personal_stats(profile_params=1) api_client.personal_stats
-(profile_params='/steam/123456789', mode='steam') api_client.personal_stats
-(profile_params=['/steam/123456789', '/steam/123456789'], mode='steam')
-api_client.personal_stats(profile_params='yoursuperalias', mode='alias')
-api_client.personal_stats(profile_params=['yoursuperalias', 'awesomealias'],
-mode='alias') ```` # Examples First of all, you'll need an APIClient instance
-to retrieve the api data: ````python import cohpy api_client =
-cohpy.get_api_client() ```` Then you could use the API interface to retrieve
-the data you want: ````python import cohpy all_leaderboards =
-api_client.leaderboards() # Returns all leaderboards info
-american_3v3_leaderboard = api_client.leaderboard
+forget to set the mode). It can be a list of ints or strings. Steam queries
+must follow /steam/[0-9]+ pattern. - mode (optional): **Default=relic** Set the
+query mode. Options are [relic, steam, alias]. - remove_server_status
+(optional): **Default=True** Remove from the response the server status
+(redundant). You can show it setting this param to **False** ````python import
+cohpy api_client = cohpy.get_api_client() api_client.personal_stats
+(profile_params=[1, 2]) api_client.personal_stats(profile_params=1)
+api_client.personal_stats(profile_params='/steam/123456789', mode='steam')
+api_client.personal_stats(profile_params=['/steam/123456789', '/steam/
+123456789'], mode='steam') api_client.personal_stats
+(profile_params='yoursuperalias', mode='alias') api_client.personal_stats
+(profile_params=['yoursuperalias', 'awesomealias'], mode='alias') ```` #
+Examples First of all, you'll need an APIClient instance to retrieve the api
+data: ````python import cohpy api_client = cohpy.get_api_client() ```` Then you
+could use the API interface to retrieve the data you want: ````python import
+cohpy all_leaderboards = api_client.leaderboards() # Returns all leaderboards
+info american_3v3_leaderboard = api_client.leaderboard
 (leaderboard_id=cohpy.Codes.USF3v3) # Returns info from specific leaderboard
 ```` Note that ````leaderboard_id```` can be a int or a cohpy.Codes instance.
```

