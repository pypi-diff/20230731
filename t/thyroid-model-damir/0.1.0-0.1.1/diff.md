# Comparing `tmp/thyroid_model_damir-0.1.0.tar.gz` & `tmp/thyroid_model_damir-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thyroid_model_damir-0.1.0.tar", last modified: Thu Jul 27 09:22:51 2023, max compression
+gzip compressed data, was "thyroid_model_damir-0.1.1.tar", last modified: Mon Jul 31 09:37:06 2023, max compression
```

## Comparing `thyroid_model_damir-0.1.0.tar` & `thyroid_model_damir-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 damirbogdan39  (1000) damirbogdan39  (1000)        0 2023-07-27 09:22:51.741186 thyroid_model_damir-0.1.0/
--rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)     1069 2023-07-27 08:37:33.000000 thyroid_model_damir-0.1.0/LICENSE
--rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)     1067 2023-07-27 09:22:51.741186 thyroid_model_damir-0.1.0/PKG-INFO
--rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)       38 2023-07-27 09:22:51.741186 thyroid_model_damir-0.1.0/setup.cfg
--rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)     1628 2023-07-27 09:22:25.000000 thyroid_model_damir-0.1.0/setup.py
-drwxrwxr-x   0 damirbogdan39  (1000) damirbogdan39  (1000)        0 2023-07-27 09:22:51.741186 thyroid_model_damir-0.1.0/thyroid_model_damir/
--rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)        0 2023-07-27 09:11:20.000000 thyroid_model_damir-0.1.0/thyroid_model_damir/__init__.py
--rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)     3454 2023-07-27 08:34:51.000000 thyroid_model_damir-0.1.0/thyroid_model_damir/create_pipeline.py
--rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)      617 2023-07-27 08:06:19.000000 thyroid_model_damir-0.1.0/thyroid_model_damir/label_encoder.joblib
--rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)      548 2023-07-27 09:19:40.000000 thyroid_model_damir-0.1.0/thyroid_model_damir/load_label_encoder.py
--rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)     1540 2023-07-27 09:22:04.000000 thyroid_model_damir-0.1.0/thyroid_model_damir/load_pipeline.py
--rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)   370174 2023-07-27 08:06:19.000000 thyroid_model_damir-0.1.0/thyroid_model_damir/pipeline.joblib
--rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)   306546 2023-07-26 09:40:01.000000 thyroid_model_damir-0.1.0/thyroid_model_damir/raw.csv
--rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)     2183 2023-07-27 08:13:13.000000 thyroid_model_damir-0.1.0/thyroid_model_damir/tests.py
-drwxrwxr-x   0 damirbogdan39  (1000) damirbogdan39  (1000)        0 2023-07-27 09:22:51.741186 thyroid_model_damir-0.1.0/thyroid_model_damir.egg-info/
--rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)     1067 2023-07-27 09:22:51.000000 thyroid_model_damir-0.1.0/thyroid_model_damir.egg-info/PKG-INFO
--rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)      514 2023-07-27 09:22:51.000000 thyroid_model_damir-0.1.0/thyroid_model_damir.egg-info/SOURCES.txt
--rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)        1 2023-07-27 09:22:51.000000 thyroid_model_damir-0.1.0/thyroid_model_damir.egg-info/dependency_links.txt
--rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)       85 2023-07-27 09:22:51.000000 thyroid_model_damir-0.1.0/thyroid_model_damir.egg-info/requires.txt
--rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)       20 2023-07-27 09:22:51.000000 thyroid_model_damir-0.1.0/thyroid_model_damir.egg-info/top_level.txt
+drwxrwxr-x   0 damirbogdan39  (1000) damirbogdan39  (1000)        0 2023-07-31 09:37:06.570226 thyroid_model_damir-0.1.1/
+-rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)     1069 2023-07-27 08:37:33.000000 thyroid_model_damir-0.1.1/LICENSE
+-rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)     1041 2023-07-31 09:37:06.570226 thyroid_model_damir-0.1.1/PKG-INFO
+-rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)       38 2023-07-31 09:37:06.570226 thyroid_model_damir-0.1.1/setup.cfg
+-rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)     1596 2023-07-31 09:36:19.000000 thyroid_model_damir-0.1.1/setup.py
+drwxrwxr-x   0 damirbogdan39  (1000) damirbogdan39  (1000)        0 2023-07-31 09:37:06.570226 thyroid_model_damir-0.1.1/thyroid_model_damir/
+-rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)        0 2023-07-27 09:11:20.000000 thyroid_model_damir-0.1.1/thyroid_model_damir/__init__.py
+-rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)     3454 2023-07-27 08:34:51.000000 thyroid_model_damir-0.1.1/thyroid_model_damir/create_pipeline.py
+-rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)      617 2023-07-27 08:06:19.000000 thyroid_model_damir-0.1.1/thyroid_model_damir/label_encoder.joblib
+-rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)      548 2023-07-27 09:19:40.000000 thyroid_model_damir-0.1.1/thyroid_model_damir/load_label_encoder.py
+-rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)     1540 2023-07-27 09:22:04.000000 thyroid_model_damir-0.1.1/thyroid_model_damir/load_pipeline.py
+-rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)   370174 2023-07-27 08:06:19.000000 thyroid_model_damir-0.1.1/thyroid_model_damir/pipeline.joblib
+-rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)   306546 2023-07-26 09:40:01.000000 thyroid_model_damir-0.1.1/thyroid_model_damir/raw.csv
+-rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)     2183 2023-07-27 08:13:13.000000 thyroid_model_damir-0.1.1/thyroid_model_damir/tests.py
+drwxrwxr-x   0 damirbogdan39  (1000) damirbogdan39  (1000)        0 2023-07-31 09:37:06.570226 thyroid_model_damir-0.1.1/thyroid_model_damir.egg-info/
+-rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)     1041 2023-07-31 09:37:06.000000 thyroid_model_damir-0.1.1/thyroid_model_damir.egg-info/PKG-INFO
+-rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)      514 2023-07-31 09:37:06.000000 thyroid_model_damir-0.1.1/thyroid_model_damir.egg-info/SOURCES.txt
+-rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)        1 2023-07-31 09:37:06.000000 thyroid_model_damir-0.1.1/thyroid_model_damir.egg-info/dependency_links.txt
+-rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)       85 2023-07-31 09:37:06.000000 thyroid_model_damir-0.1.1/thyroid_model_damir.egg-info/requires.txt
+-rw-rw-r--   0 damirbogdan39  (1000) damirbogdan39  (1000)       20 2023-07-31 09:37:06.000000 thyroid_model_damir-0.1.1/thyroid_model_damir.egg-info/top_level.txt
```

### Comparing `thyroid_model_damir-0.1.0/LICENSE` & `thyroid_model_damir-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thyroid_model_damir-0.1.0/PKG-INFO` & `thyroid_model_damir-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: thyroid_model_damir
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pretrained thyroid model and pipeline for classification
 Author: Damir Bogdan
 Author-email: damribogdan39@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 Thyroid classification package 
 
 This package contains a sklearn pipeline that incorporates necessary preprocessing steps and a XGBoost classification model
```

### Comparing `thyroid_model_damir-0.1.0/setup.py` & `thyroid_model_damir-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,28 +24,27 @@
 # To predict use:
 y_pred = pipeline.predict(X) # X is a dataframe object of features
 y_encoded = encoder.inverse_transform(y_pred)
 ```
 """
 setup(
     name='thyroid_model_damir',
-    version='0.1.0',
+    version='0.1.1',
     author='Damir Bogdan',
     author_email='damribogdan39@gmail.com',
     description='Pretrained thyroid model and pipeline for classification',
     long_description=description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     package_data={'thyroid_model_damir': ['pipeline.joblib', 'label_encoder.joblib', 'raw.csv']},
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.10.6',
     install_requires=[  
         'numpy==1.25.0',
         'scikit-learn==1.0.2',
         'xgboost==1.7.6',
         'pandas==1.5.3',
         'joblib==1.3.1',
         'pathlib'
```

### Comparing `thyroid_model_damir-0.1.0/thyroid_model_damir/create_pipeline.py` & `thyroid_model_damir-0.1.1/thyroid_model_damir/create_pipeline.py`

 * *Files identical despite different names*

### Comparing `thyroid_model_damir-0.1.0/thyroid_model_damir/label_encoder.joblib` & `thyroid_model_damir-0.1.1/thyroid_model_damir/label_encoder.joblib`

 * *Files identical despite different names*

### Comparing `thyroid_model_damir-0.1.0/thyroid_model_damir/load_label_encoder.py` & `thyroid_model_damir-0.1.1/thyroid_model_damir/load_label_encoder.py`

 * *Files identical despite different names*

### Comparing `thyroid_model_damir-0.1.0/thyroid_model_damir/load_pipeline.py` & `thyroid_model_damir-0.1.1/thyroid_model_damir/load_pipeline.py`

 * *Files identical despite different names*

### Comparing `thyroid_model_damir-0.1.0/thyroid_model_damir/pipeline.joblib` & `thyroid_model_damir-0.1.1/thyroid_model_damir/pipeline.joblib`

 * *Files identical despite different names*

### Comparing `thyroid_model_damir-0.1.0/thyroid_model_damir/raw.csv` & `thyroid_model_damir-0.1.1/thyroid_model_damir/raw.csv`

 * *Files identical despite different names*

### Comparing `thyroid_model_damir-0.1.0/thyroid_model_damir/tests.py` & `thyroid_model_damir-0.1.1/thyroid_model_damir/tests.py`

 * *Files identical despite different names*

### Comparing `thyroid_model_damir-0.1.0/thyroid_model_damir.egg-info/PKG-INFO` & `thyroid_model_damir-0.1.1/thyroid_model_damir.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: thyroid-model-damir
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pretrained thyroid model and pipeline for classification
 Author: Damir Bogdan
 Author-email: damribogdan39@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 Thyroid classification package 
 
 This package contains a sklearn pipeline that incorporates necessary preprocessing steps and a XGBoost classification model
```

### Comparing `thyroid_model_damir-0.1.0/thyroid_model_damir.egg-info/SOURCES.txt` & `thyroid_model_damir-0.1.1/thyroid_model_damir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

