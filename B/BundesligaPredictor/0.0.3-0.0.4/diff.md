# Comparing `tmp/BundesligaPredictor-0.0.3.tar.gz` & `tmp/BundesligaPredictor-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BundesligaPredictor-0.0.3.tar", last modified: Mon Jul 31 09:11:39 2023, max compression
+gzip compressed data, was "BundesligaPredictor-0.0.4.tar", last modified: Mon Jul 31 10:03:30 2023, max compression
```

## Comparing `BundesligaPredictor-0.0.3.tar` & `BundesligaPredictor-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 09:11:39.287201 BundesligaPredictor-0.0.3/
-drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 09:11:39.278313 BundesligaPredictor-0.0.3/BundesligaPredictor.egg-info/
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)       63 2023-07-31 09:11:39.000000 BundesligaPredictor-0.0.3/BundesligaPredictor.egg-info/PKG-INFO
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)      489 2023-07-31 09:11:39.000000 BundesligaPredictor-0.0.3/BundesligaPredictor.egg-info/SOURCES.txt
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)        1 2023-07-31 09:11:39.000000 BundesligaPredictor-0.0.3/BundesligaPredictor.egg-info/dependency_links.txt
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)       54 2023-07-31 09:11:39.000000 BundesligaPredictor-0.0.3/BundesligaPredictor.egg-info/requires.txt
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)       14 2023-07-31 09:11:39.000000 BundesligaPredictor-0.0.3/BundesligaPredictor.egg-info/top_level.txt
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)       63 2023-07-31 09:11:39.287049 BundesligaPredictor-0.0.3/PKG-INFO
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)        0 2023-07-30 13:53:47.000000 BundesligaPredictor-0.0.3/README.md
-drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 09:11:39.280118 BundesligaPredictor-0.0.3/scripts/
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)        0 2023-07-30 06:11:22.000000 BundesligaPredictor-0.0.3/scripts/__init__.py
-drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 09:11:39.283906 BundesligaPredictor-0.0.3/scripts/data/
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)  2545843 2023-07-30 16:30:55.000000 BundesligaPredictor-0.0.3/scripts/data/germany_all.csv
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)   167237 2023-07-31 06:37:16.000000 BundesligaPredictor-0.0.3/scripts/data/preprocessed_data.csv
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)      101 2023-07-30 17:06:01.000000 BundesligaPredictor-0.0.3/scripts/load.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)     1993 2023-07-31 09:05:32.000000 BundesligaPredictor-0.0.3/scripts/pre_process.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)     1858 2023-07-31 06:50:48.000000 BundesligaPredictor-0.0.3/scripts/scraper.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)      719 2023-07-30 17:04:47.000000 BundesligaPredictor-0.0.3/scripts/serve.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)      261 2023-07-31 07:15:30.000000 BundesligaPredictor-0.0.3/scripts/test.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)     2335 2023-07-31 06:51:10.000000 BundesligaPredictor-0.0.3/scripts/train.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)       38 2023-07-31 09:11:39.287243 BundesligaPredictor-0.0.3/setup.cfg
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)      370 2023-07-31 09:11:37.000000 BundesligaPredictor-0.0.3/setup.py
-drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 09:11:39.286639 BundesligaPredictor-0.0.3/tests/
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)        0 2023-07-30 13:41:35.000000 BundesligaPredictor-0.0.3/tests/__init__.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)     1479 2023-07-31 09:09:05.000000 BundesligaPredictor-0.0.3/tests/preprocess_test.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)      419 2023-07-31 07:13:10.000000 BundesligaPredictor-0.0.3/tests/scraper_test.py
+drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 10:03:30.793758 BundesligaPredictor-0.0.4/
+drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 10:03:30.783847 BundesligaPredictor-0.0.4/BundesligaPredictor.egg-info/
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)       63 2023-07-31 10:03:30.000000 BundesligaPredictor-0.0.4/BundesligaPredictor.egg-info/PKG-INFO
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)      453 2023-07-31 10:03:30.000000 BundesligaPredictor-0.0.4/BundesligaPredictor.egg-info/SOURCES.txt
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)        1 2023-07-31 10:03:30.000000 BundesligaPredictor-0.0.4/BundesligaPredictor.egg-info/dependency_links.txt
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)       54 2023-07-31 10:03:30.000000 BundesligaPredictor-0.0.4/BundesligaPredictor.egg-info/requires.txt
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)       14 2023-07-31 10:03:30.000000 BundesligaPredictor-0.0.4/BundesligaPredictor.egg-info/top_level.txt
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)       63 2023-07-31 10:03:30.793596 BundesligaPredictor-0.0.4/PKG-INFO
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)        0 2023-07-30 13:53:47.000000 BundesligaPredictor-0.0.4/README.md
+drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 10:03:30.786385 BundesligaPredictor-0.0.4/scripts/
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)        0 2023-07-30 06:11:22.000000 BundesligaPredictor-0.0.4/scripts/__init__.py
+drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 10:03:30.786783 BundesligaPredictor-0.0.4/scripts/data/
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)  2545843 2023-07-30 16:30:55.000000 BundesligaPredictor-0.0.4/scripts/data/germany_all.csv
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)      101 2023-07-30 17:06:01.000000 BundesligaPredictor-0.0.4/scripts/load.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)     1987 2023-07-31 09:39:04.000000 BundesligaPredictor-0.0.4/scripts/preprocess.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)     1858 2023-07-31 06:50:48.000000 BundesligaPredictor-0.0.4/scripts/scraper.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)      719 2023-07-30 17:04:47.000000 BundesligaPredictor-0.0.4/scripts/serve.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)      261 2023-07-31 07:15:30.000000 BundesligaPredictor-0.0.4/scripts/test.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)     2335 2023-07-31 06:51:10.000000 BundesligaPredictor-0.0.4/scripts/train.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)       38 2023-07-31 10:03:30.793803 BundesligaPredictor-0.0.4/setup.cfg
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)      370 2023-07-31 10:03:26.000000 BundesligaPredictor-0.0.4/setup.py
+drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 10:03:30.792365 BundesligaPredictor-0.0.4/tests/
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)        0 2023-07-30 13:41:35.000000 BundesligaPredictor-0.0.4/tests/__init__.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)     1471 2023-07-31 10:00:22.000000 BundesligaPredictor-0.0.4/tests/preprocess_test.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)      427 2023-07-31 10:00:29.000000 BundesligaPredictor-0.0.4/tests/scraper_test.py
```

### Comparing `BundesligaPredictor-0.0.3/scripts/data/germany_all.csv` & `BundesligaPredictor-0.0.4/scripts/data/germany_all.csv`

 * *Files identical despite different names*

### Comparing `BundesligaPredictor-0.0.3/scripts/pre_process.py` & `BundesligaPredictor-0.0.4/scripts/preprocess.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import pandas as pd
 from sklearn.preprocessing import LabelEncoder
 
 class FootballDataPreprocessor:
+    '''
+    Preprocess the football data.
+    
+    '''
 
     def __init__(self, dataframe):
         self.dataframe = dataframe
         self.team_encoder = LabelEncoder()
         self.teams = {0: 'Aalen', 1: 'Augsburg', 2: 'Bayern Munich', 3: 'Bielefeld', 4: 'Bochum', 5: 'Braunschweig',
                       6: 'Cottbus', 7: 'Darmstadt', 8: 'Dortmund', 9: 'Dresden', 10: 'Duisburg', 11: 'Ein Frankfurt',
                       12: 'Erzgebirge Aue', 13: 'FC Koln', 14: 'Fortuna Dusseldorf', 15: 'Frankfurt FSV', 16: 'Freiburg', 
@@ -14,20 +18,15 @@
                       27: 'Leverkusen', 28: "M'gladbach", 29: 'Magdeburg', 30: 'Mainz', 31: 'Munich 1860', 32: 'Nurnberg', 
                       33: 'Paderborn', 34: 'RB Leipzig', 35: 'Regensburg', 36: 'Sandhausen', 37: 'Schalke 04', 
                       38: 'St Pauli', 39: 'Stuttgart', 40: 'Union Berlin', 41: 'Werder Bremen', 42: 'Wolfsburg', 
                       43: 'Wurzburger Kickers'}
 
     def preprocess(self):
         # Select the relevant columns
-        relevant_cols = [
-            'Div', 'HomeTeam', 'AwayTeam',
-            'B365H', 'B365D', 'B365A', 
-            'BbAv<2.5', 'BbAv>2.5', 
-            'BbAvAHH', 'BbAvAHA',
-        ]
+        relevant_cols = ['HomeTeam', 'AwayTeam', 'B365H', 'B365D', 'B365A', 'BbAv<2.5', 'BbAv>2.5', 'BbAvAHH', 'BbAvAHA', 'Div']
         df = self.dataframe[relevant_cols]
 
         # Drop rows with missing values
         df = df.dropna()
 
         # Use the params to encode the 'HomeTeam' and 'AwayTeam' columns
         self.team_encoder.fit(sorted(list(self.teams.values())))
```

### Comparing `BundesligaPredictor-0.0.3/scripts/scraper.py` & `BundesligaPredictor-0.0.4/scripts/scraper.py`

 * *Files identical despite different names*

### Comparing `BundesligaPredictor-0.0.3/scripts/serve.py` & `BundesligaPredictor-0.0.4/scripts/serve.py`

 * *Files identical despite different names*

### Comparing `BundesligaPredictor-0.0.3/scripts/train.py` & `BundesligaPredictor-0.0.4/scripts/train.py`

 * *Files identical despite different names*

### Comparing `BundesligaPredictor-0.0.3/tests/preprocess_test.py` & `BundesligaPredictor-0.0.4/tests/preprocess_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
-from scripts.pre_process import FootballDataPreprocessor
 import pandas as pd
 import numpy as np
+from package.scripts.preprocess import FootballDataPreprocessor
 
 class TestFootballDataPreprocessor(unittest.TestCase):
 
     def setUp(self):
         self.data = pd.DataFrame({
             'Div': ['D1', 'D2', 'D1'],
             'HomeTeam': ['Aalen', 'Augsburg', 'Bayern Munich'],
@@ -24,18 +24,16 @@
     def test_preprocess(self):
         processed_data = self.processor.preprocess()
 
         # Check if the output DataFrame has the right shape
         self.assertEqual(processed_data.shape, self.data.shape)
 
         # Check if the output DataFrame has the right columns
-        expected_columns = ['HomeTeam', 'AwayTeam', 'B365H', 'B365D', 'B365A', 'BbAv<2.5', 'BbAv>2.5', 'BbAvAHH', 'BbAvAHA', 'Div']
+        expected_columns = ['Div', 'HomeTeam', 'AwayTeam', 'B365H', 'B365D', 'B365A', 'BbAv<2.5', 'BbAv>2.5', 'BbAvAHH', 'BbAvAHA']
         self.assertSetEqual(set(processed_data.columns), set(expected_columns))
 
-        # Check if the 'Div_B' column has been correctly created
-        expected_div_b = np.array([0, 1, 0])
-        np.testing.assert_array_equal(processed_data['Div'].values, expected_div_b)
-
-        
+        # Check if the 'Div' column has been correctly created
+        expected_div = np.array([0, 1, 0])
+        np.testing.assert_array_equal(processed_data['Div'].values, expected_div)
 
 if __name__ == '__main__':
-    unittest.main()
+    unittest.main()
```

