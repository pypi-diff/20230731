# Comparing `tmp/BundesligaPredictor-0.0.2.tar.gz` & `tmp/BundesligaPredictor-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BundesligaPredictor-0.0.2.tar", last modified: Mon Jul 31 07:08:14 2023, max compression
+gzip compressed data, was "BundesligaPredictor-0.0.3.tar", last modified: Mon Jul 31 09:11:39 2023, max compression
```

## Comparing `BundesligaPredictor-0.0.2.tar` & `BundesligaPredictor-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 07:08:14.285759 BundesligaPredictor-0.0.2/
-drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 07:08:14.272060 BundesligaPredictor-0.0.2/BundesligaPredictor.egg-info/
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)       63 2023-07-31 07:08:14.000000 BundesligaPredictor-0.0.2/BundesligaPredictor.egg-info/PKG-INFO
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)      489 2023-07-31 07:08:14.000000 BundesligaPredictor-0.0.2/BundesligaPredictor.egg-info/SOURCES.txt
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)        1 2023-07-31 07:08:14.000000 BundesligaPredictor-0.0.2/BundesligaPredictor.egg-info/dependency_links.txt
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)       54 2023-07-31 07:08:14.000000 BundesligaPredictor-0.0.2/BundesligaPredictor.egg-info/requires.txt
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)       14 2023-07-31 07:08:14.000000 BundesligaPredictor-0.0.2/BundesligaPredictor.egg-info/top_level.txt
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)       63 2023-07-31 07:08:14.285461 BundesligaPredictor-0.0.2/PKG-INFO
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)        0 2023-07-30 13:53:47.000000 BundesligaPredictor-0.0.2/README.md
-drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 07:08:14.274000 BundesligaPredictor-0.0.2/scripts/
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)        0 2023-07-30 06:11:22.000000 BundesligaPredictor-0.0.2/scripts/__init__.py
-drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 07:08:14.279321 BundesligaPredictor-0.0.2/scripts/data/
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)  2545843 2023-07-30 16:30:55.000000 BundesligaPredictor-0.0.2/scripts/data/germany_all.csv
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)   167237 2023-07-31 06:37:16.000000 BundesligaPredictor-0.0.2/scripts/data/preprocessed_data.csv
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)      101 2023-07-30 17:06:01.000000 BundesligaPredictor-0.0.2/scripts/load.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)     1989 2023-07-31 06:45:32.000000 BundesligaPredictor-0.0.2/scripts/pre_process.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)     1858 2023-07-31 06:50:48.000000 BundesligaPredictor-0.0.2/scripts/scraper.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)      719 2023-07-30 17:04:47.000000 BundesligaPredictor-0.0.2/scripts/serve.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)     1851 2023-07-31 06:37:13.000000 BundesligaPredictor-0.0.2/scripts/test.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)     2335 2023-07-31 06:51:10.000000 BundesligaPredictor-0.0.2/scripts/train.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)       38 2023-07-31 07:08:14.285811 BundesligaPredictor-0.0.2/setup.cfg
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)      370 2023-07-31 07:06:43.000000 BundesligaPredictor-0.0.2/setup.py
-drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 07:08:14.285199 BundesligaPredictor-0.0.2/tests/
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)        0 2023-07-30 13:41:35.000000 BundesligaPredictor-0.0.2/tests/__init__.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)     1509 2023-07-31 06:58:23.000000 BundesligaPredictor-0.0.2/tests/preprocess_test.py
--rw-r--r--   0 davitgamtenadze   (501) staff       (20)      419 2023-07-30 13:47:19.000000 BundesligaPredictor-0.0.2/tests/scraper_test.py
+drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 09:11:39.287201 BundesligaPredictor-0.0.3/
+drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 09:11:39.278313 BundesligaPredictor-0.0.3/BundesligaPredictor.egg-info/
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)       63 2023-07-31 09:11:39.000000 BundesligaPredictor-0.0.3/BundesligaPredictor.egg-info/PKG-INFO
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)      489 2023-07-31 09:11:39.000000 BundesligaPredictor-0.0.3/BundesligaPredictor.egg-info/SOURCES.txt
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)        1 2023-07-31 09:11:39.000000 BundesligaPredictor-0.0.3/BundesligaPredictor.egg-info/dependency_links.txt
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)       54 2023-07-31 09:11:39.000000 BundesligaPredictor-0.0.3/BundesligaPredictor.egg-info/requires.txt
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)       14 2023-07-31 09:11:39.000000 BundesligaPredictor-0.0.3/BundesligaPredictor.egg-info/top_level.txt
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)       63 2023-07-31 09:11:39.287049 BundesligaPredictor-0.0.3/PKG-INFO
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)        0 2023-07-30 13:53:47.000000 BundesligaPredictor-0.0.3/README.md
+drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 09:11:39.280118 BundesligaPredictor-0.0.3/scripts/
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)        0 2023-07-30 06:11:22.000000 BundesligaPredictor-0.0.3/scripts/__init__.py
+drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 09:11:39.283906 BundesligaPredictor-0.0.3/scripts/data/
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)  2545843 2023-07-30 16:30:55.000000 BundesligaPredictor-0.0.3/scripts/data/germany_all.csv
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)   167237 2023-07-31 06:37:16.000000 BundesligaPredictor-0.0.3/scripts/data/preprocessed_data.csv
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)      101 2023-07-30 17:06:01.000000 BundesligaPredictor-0.0.3/scripts/load.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)     1993 2023-07-31 09:05:32.000000 BundesligaPredictor-0.0.3/scripts/pre_process.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)     1858 2023-07-31 06:50:48.000000 BundesligaPredictor-0.0.3/scripts/scraper.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)      719 2023-07-30 17:04:47.000000 BundesligaPredictor-0.0.3/scripts/serve.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)      261 2023-07-31 07:15:30.000000 BundesligaPredictor-0.0.3/scripts/test.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)     2335 2023-07-31 06:51:10.000000 BundesligaPredictor-0.0.3/scripts/train.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)       38 2023-07-31 09:11:39.287243 BundesligaPredictor-0.0.3/setup.cfg
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)      370 2023-07-31 09:11:37.000000 BundesligaPredictor-0.0.3/setup.py
+drwxr-xr-x   0 davitgamtenadze   (501) staff       (20)        0 2023-07-31 09:11:39.286639 BundesligaPredictor-0.0.3/tests/
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)        0 2023-07-30 13:41:35.000000 BundesligaPredictor-0.0.3/tests/__init__.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)     1479 2023-07-31 09:09:05.000000 BundesligaPredictor-0.0.3/tests/preprocess_test.py
+-rw-r--r--   0 davitgamtenadze   (501) staff       (20)      419 2023-07-31 07:13:10.000000 BundesligaPredictor-0.0.3/tests/scraper_test.py
```

### Comparing `BundesligaPredictor-0.0.2/scripts/data/germany_all.csv` & `BundesligaPredictor-0.0.3/scripts/data/germany_all.csv`

 * *Files identical despite different names*

### Comparing `BundesligaPredictor-0.0.2/scripts/data/preprocessed_data.csv` & `BundesligaPredictor-0.0.3/scripts/data/preprocessed_data.csv`

 * *Files identical despite different names*

### Comparing `BundesligaPredictor-0.0.2/scripts/pre_process.py` & `BundesligaPredictor-0.0.3/scripts/pre_process.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,23 +18,23 @@
 
     def preprocess(self):
         # Select the relevant columns
         relevant_cols = [
             'Div', 'HomeTeam', 'AwayTeam',
             'B365H', 'B365D', 'B365A', 
             'BbAv<2.5', 'BbAv>2.5', 
-            'BbAvAHH', 'BbAvAHA', 'FTR'
+            'BbAvAHH', 'BbAvAHA',
         ]
         df = self.dataframe[relevant_cols]
 
         # Drop rows with missing values
         df = df.dropna()
 
         # Use the params to encode the 'HomeTeam' and 'AwayTeam' columns
         self.team_encoder.fit(sorted(list(self.teams.values())))
         df['HomeTeam'] = self.team_encoder.transform(df['HomeTeam'])
         df['AwayTeam'] = self.team_encoder.transform(df['AwayTeam'])
 
-        # Encode 'Div' column, without creating new columns
-        df = pd.get_dummies(df, columns=['Div'], drop_first=True)
-
+        # Encode div manuallt 1 if Div = D1, 0 if Div = D2
+        df['Div'] = df['Div'].apply(lambda x: 1 if x == 'D2' else 0)
+        
         return df
```

### Comparing `BundesligaPredictor-0.0.2/scripts/scraper.py` & `BundesligaPredictor-0.0.3/scripts/scraper.py`

 * *Files identical despite different names*

### Comparing `BundesligaPredictor-0.0.2/scripts/serve.py` & `BundesligaPredictor-0.0.3/scripts/serve.py`

 * *Files identical despite different names*

### Comparing `BundesligaPredictor-0.0.2/scripts/train.py` & `BundesligaPredictor-0.0.3/scripts/train.py`

 * *Files identical despite different names*

### Comparing `BundesligaPredictor-0.0.2/tests/preprocess_test.py` & `BundesligaPredictor-0.0.3/tests/preprocess_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,38 +3,39 @@
 import pandas as pd
 import numpy as np
 
 class TestFootballDataPreprocessor(unittest.TestCase):
 
     def setUp(self):
         self.data = pd.DataFrame({
-            'Div': ['A', 'A', 'B'],
+            'Div': ['D1', 'D2', 'D1'],
             'HomeTeam': ['Aalen', 'Augsburg', 'Bayern Munich'],
             'AwayTeam': ['Bielefeld', 'Bochum', 'Braunschweig'],
             'B365H': [1.5, 2.3, 3.4],
             'B365D': [2.4, 3.2, 2.1],
             'B365A': [2.5, 3.4, 2.2],
             'BbAv<2.5': [1.6, 2.7, 1.8],
             'BbAv>2.5': [2.6, 3.8, 2.9],
             'BbAvAHH': [1.7, 2.8, 1.9],
             'BbAvAHA': [2.7, 3.9, 2.1],
-            'FTR': ['H', 'A', 'D']
         })
 
         self.processor = FootballDataPreprocessor(self.data)
 
     def test_preprocess(self):
         processed_data = self.processor.preprocess()
 
         # Check if the output DataFrame has the right shape
         self.assertEqual(processed_data.shape, self.data.shape)
 
         # Check if the output DataFrame has the right columns
-        expected_columns = ['HomeTeam', 'AwayTeam', 'FTR', 'B365H', 'B365D', 'B365A', 'BbAv<2.5', 'BbAv>2.5', 'BbAvAHH', 'BbAvAHA', 'Div_B']
-        self.assertListEqual(list(processed_data.columns), expected_columns)
+        expected_columns = ['HomeTeam', 'AwayTeam', 'B365H', 'B365D', 'B365A', 'BbAv<2.5', 'BbAv>2.5', 'BbAvAHH', 'BbAvAHA', 'Div']
+        self.assertSetEqual(set(processed_data.columns), set(expected_columns))
 
         # Check if the 'Div_B' column has been correctly created
-        expected_div_b = np.array([0, 0, 1])
-        np.testing.assert_array_equal(processed_data['Div_B'].values, expected_div_b)
+        expected_div_b = np.array([0, 1, 0])
+        np.testing.assert_array_equal(processed_data['Div'].values, expected_div_b)
+
+        
 
 if __name__ == '__main__':
     unittest.main()
```

