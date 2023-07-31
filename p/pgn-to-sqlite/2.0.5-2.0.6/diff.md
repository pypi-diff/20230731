# Comparing `tmp/pgn_to_sqlite-2.0.5.tar.gz` & `tmp/pgn_to_sqlite-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgn_to_sqlite-2.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pgn_to_sqlite-2.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pgn_to_sqlite-2.0.5.tar` & `pgn_to_sqlite-2.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       54 2023-05-23 21:46:10.993140 pgn_to_sqlite-2.0.5/.coveragerc
--rw-r--r--   0        0        0      620 2023-05-23 21:46:10.993140 pgn_to_sqlite-2.0.5/.github/workflows/publish.yml
--rw-r--r--   0        0        0      694 2023-05-23 21:46:10.993140 pgn_to_sqlite-2.0.5/.github/workflows/run_tests.yml
--rw-r--r--   0        0        0       84 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/.gitignore
--rw-r--r--   0        0        0     1078 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/LICENSE
--rw-r--r--   0        0        0     2867 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/README.md
--rw-r--r--   0        0        0      111 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/pgn_to_sqlite/__init__.py
--rw-r--r--   0        0        0     8071 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/pgn_to_sqlite/cli.py
--rw-r--r--   0        0        0      919 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/pyproject.toml
--rw-r--r--   0        0        0      155 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/pytest.ini
--rw-r--r--   0        0        0      265 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/requirements.in
--rw-r--r--   0        0        0    22534 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/tests/__init__.py
--rw-r--r--   0        0        0      506 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/tests/game_files/test_pgn_file_chess_dotcom.pgn
--rw-r--r--   0        0        0      885 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/tests/game_files/test_pgn_file_lichess.pgn
--rw-r--r--   0        0        0     1369 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/tests/test_cli.py
--rw-r--r--   0        0        0      159 2023-05-23 21:46:10.997140 pgn_to_sqlite-2.0.5/tox.ini
--rw-r--r--   0        0        0     3757 1970-01-01 00:00:00.000000 pgn_to_sqlite-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0       54 2023-07-31 18:44:41.017299 pgn_to_sqlite-2.0.6/.coveragerc
+-rw-r--r--   0        0        0      620 2023-07-31 18:44:41.017299 pgn_to_sqlite-2.0.6/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      694 2023-07-31 18:44:41.017299 pgn_to_sqlite-2.0.6/.github/workflows/run_tests.yml
+-rw-r--r--   0        0        0       84 2023-07-31 18:44:41.017299 pgn_to_sqlite-2.0.6/.gitignore
+-rw-r--r--   0        0        0     1078 2023-07-31 18:44:41.017299 pgn_to_sqlite-2.0.6/LICENSE
+-rw-r--r--   0        0        0     2867 2023-07-31 18:44:41.017299 pgn_to_sqlite-2.0.6/README.md
+-rw-r--r--   0        0        0      111 2023-07-31 18:44:41.017299 pgn_to_sqlite-2.0.6/pgn_to_sqlite/__init__.py
+-rw-r--r--   0        0        0     8071 2023-07-31 18:44:41.017299 pgn_to_sqlite-2.0.6/pgn_to_sqlite/cli.py
+-rw-r--r--   0        0        0      919 2023-07-31 18:44:41.017299 pgn_to_sqlite-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0      155 2023-07-31 18:44:41.017299 pgn_to_sqlite-2.0.6/pytest.ini
+-rw-r--r--   0        0        0      265 2023-07-31 18:44:41.017299 pgn_to_sqlite-2.0.6/requirements.in
+-rw-r--r--   0        0        0    22534 2023-07-31 18:44:41.017299 pgn_to_sqlite-2.0.6/requirements.txt
+-rw-r--r--   0        0        0        0 2023-07-31 18:44:41.017299 pgn_to_sqlite-2.0.6/tests/__init__.py
+-rw-r--r--   0        0        0      506 2023-07-31 18:44:41.017299 pgn_to_sqlite-2.0.6/tests/game_files/test_pgn_file_chess_dotcom.pgn
+-rw-r--r--   0        0        0      885 2023-07-31 18:44:41.017299 pgn_to_sqlite-2.0.6/tests/game_files/test_pgn_file_lichess.pgn
+-rw-r--r--   0        0        0     1369 2023-07-31 18:44:41.017299 pgn_to_sqlite-2.0.6/tests/test_cli.py
+-rw-r--r--   0        0        0      159 2023-07-31 18:44:41.021299 pgn_to_sqlite-2.0.6/tox.ini
+-rw-r--r--   0        0        0     3757 1970-01-01 00:00:00.000000 pgn_to_sqlite-2.0.6/PKG-INFO
```

### Comparing `pgn_to_sqlite-2.0.5/.github/workflows/publish.yml` & `pgn_to_sqlite-2.0.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.0.5/.github/workflows/run_tests.yml` & `pgn_to_sqlite-2.0.6/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.0.5/LICENSE` & `pgn_to_sqlite-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.0.5/README.md` & `pgn_to_sqlite-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.0.5/pgn_to_sqlite/cli.py` & `pgn_to_sqlite-2.0.6/pgn_to_sqlite/cli.py`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.0.5/pyproject.toml` & `pgn_to_sqlite-2.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.0.5/requirements.txt` & `pgn_to_sqlite-2.0.6/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,17 @@
     --hash=sha256:974308c58d057a651d182208a484ce80a26dac0caef2895836a92dd6ebd725e0 \
     --hash=sha256:b8b49776299fece66bffaafe357d929ca9451450f5466e997a7285ab0fe28e3b \
     --hash=sha256:c957b2b4ea88587b46cf49d1dc17681c1e672864fd7af32fc1e9664d572b3458 \
     --hash=sha256:e41a86c6c650bcecc6633ee3180d80a025db041a8e2398dcc059b3afa8382cd4 \
     --hash=sha256:f513588da599943e0cde4e32cc9879e825d58720d6557062d1098c5ad80080e1 \
     --hash=sha256:fba8a281e570adafb79f7755ac8721b6cf1bbf691186a287e990c7929c7692ff
     # via -r requirements.in
-certifi==2022.12.7 \
-    --hash=sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3 \
-    --hash=sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18
+certifi==2023.7.22 \
+    --hash=sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082 \
+    --hash=sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9
     # via requests
 charset-normalizer==2.1.1 \
     --hash=sha256:5a3d016c7c547f69d6f81fb0db9449ce888b418b5b9952cc5e6e66843e9dd845 \
     --hash=sha256:83e9a75d1911279afd89352c68b45348559d1fc0506b054b346651b5e7fee29f
     # via requests
 click==8.1.3 \
     --hash=sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e \
```

### Comparing `pgn_to_sqlite-2.0.5/tests/game_files/test_pgn_file_lichess.pgn` & `pgn_to_sqlite-2.0.6/tests/game_files/test_pgn_file_lichess.pgn`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.0.5/tests/test_cli.py` & `pgn_to_sqlite-2.0.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.0.5/PKG-INFO` & `pgn_to_sqlite-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgn_to_sqlite
-Version: 2.0.5
+Version: 2.0.6
 Summary: Fetch your games from chess.com and lichess.org and add them to a sqlite database
 Home-page: https://github.com/EndlessTrax/pgn-to-sqlite
 Author: Ricky White
 Author-email: ricky@whitelionmedia.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
```

