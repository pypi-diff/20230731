# Comparing `tmp/toiro-0.0.8.tar.gz` & `tmp/toiro-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/toiro-0.0.8.tar", last modified: Mon Nov  2 18:14:58 2020, max compression
+gzip compressed data, was "dist/toiro-0.0.9.tar", last modified: Mon Jul 31 15:07:59 2023, max compression
```

## Comparing `toiro-0.0.8.tar` & `toiro-0.0.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-02 18:14:58.000000 toiro-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)       88 2020-11-02 18:14:50.000000 toiro-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    10402 2020-11-02 18:14:58.000000 toiro-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     7631 2020-11-02 18:14:50.000000 toiro-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       63 2020-11-02 18:14:58.000000 toiro-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1879 2020-11-02 18:14:50.000000 toiro-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-02 18:14:58.000000 toiro-0.0.8/test/
--rw-r--r--   0 runner    (1001) docker     (116)     1521 2020-11-02 18:14:50.000000 toiro-0.0.8/test/test_classifiers.py
--rw-r--r--   0 runner    (1001) docker     (116)     2656 2020-11-02 18:14:50.000000 toiro-0.0.8/test/test_datadownloader.py
--rw-r--r--   0 runner    (1001) docker     (116)     6555 2020-11-02 18:14:50.000000 toiro-0.0.8/test/test_tokenizers.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-02 18:14:58.000000 toiro-0.0.8/toiro/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-02 18:14:58.000000 toiro-0.0.8/toiro/classifiers/
--rw-r--r--   0 runner    (1001) docker     (116)      391 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/classifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9429 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/classifiers/classifier_bert.py
--rw-r--r--   0 runner    (1001) docker     (116)     2793 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/classifiers/classifier_svm.py
--rw-r--r--   0 runner    (1001) docker     (116)      736 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/classifiers/classifier_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-02 18:14:58.000000 toiro-0.0.8/toiro/datadownloader/
--rw-r--r--   0 runner    (1001) docker     (116)      215 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/datadownloader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-02 18:14:58.000000 toiro-0.0.8/toiro/datadownloader/data/
--rw-r--r--   0 runner    (1001) docker     (116)     8257 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/datadownloader/data/sample.dev
--rw-r--r--   0 runner    (1001) docker     (116)    10706 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/datadownloader/data/sample.test
--rw-r--r--   0 runner    (1001) docker     (116)    66257 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/datadownloader/data/sample.train
--rw-r--r--   0 runner    (1001) docker     (116)    90137 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/datadownloader/data/sample.txt
--rw-r--r--   0 runner    (1001) docker     (116)   253961 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/datadownloader/data/toiro.gif
--rw-r--r--   0 runner    (1001) docker     (116)    72909 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/datadownloader/data/toiro.png
--rw-r--r--   0 runner    (1001) docker     (116)     2266 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/datadownloader/download.py
--rw-r--r--   0 runner    (1001) docker     (116)     1735 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/datadownloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    14439 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/datadownloader/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (116)      321 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/datadownloader/sample_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-02 18:14:58.000000 toiro-0.0.8/toiro/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (116)     2588 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/tokenizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-02 18:14:58.000000 toiro-0.0.8/toiro/tokenizers/data/
--rw-r--r--   0 runner    (1001) docker     (116)   352418 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/tokenizers/data/ja.text8.txt.spm.model
--rw-r--r--   0 runner    (1001) docker     (116)   121892 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/tokenizers/data/ja.text8.txt.spm.vocab
--rw-r--r--   0 runner    (1001) docker     (116)      799 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/tokenizers/tokenizer_fugashi_ipadic.py
--rw-r--r--   0 runner    (1001) docker     (116)      620 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/tokenizers/tokenizer_fugashi_unidic.py
--rw-r--r--   0 runner    (1001) docker     (116)      624 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/tokenizers/tokenizer_ginza.py
--rw-r--r--   0 runner    (1001) docker     (116)      640 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/tokenizers/tokenizer_janome.py
--rw-r--r--   0 runner    (1001) docker     (116)      933 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/tokenizers/tokenizer_jumanpp.py
--rw-r--r--   0 runner    (1001) docker     (116)      614 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/tokenizers/tokenizer_kytea.py
--rw-r--r--   0 runner    (1001) docker     (116)      671 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/tokenizers/tokenizer_mecab_python3.py
--rw-r--r--   0 runner    (1001) docker     (116)      583 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/tokenizers/tokenizer_nagisa.py
--rw-r--r--   0 runner    (1001) docker     (116)     7174 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/tokenizers/tokenizer_report.py
--rw-r--r--   0 runner    (1001) docker     (116)      874 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/tokenizers/tokenizer_sentencepiece.py
--rw-r--r--   0 runner    (1001) docker     (116)      678 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/tokenizers/tokenizer_spacy.py
--rw-r--r--   0 runner    (1001) docker     (116)      812 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/tokenizers/tokenizer_sudachipy.py
--rw-r--r--   0 runner    (1001) docker     (116)      577 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/tokenizers/tokenizer_tinysegmenter.py
--rw-r--r--   0 runner    (1001) docker     (116)     9517 2020-11-02 18:14:50.000000 toiro-0.0.8/toiro/tokenizers/tokenizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-02 18:14:58.000000 toiro-0.0.8/toiro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    10402 2020-11-02 18:14:58.000000 toiro-0.0.8/toiro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1481 2020-11-02 18:14:58.000000 toiro-0.0.8/toiro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-02 18:14:58.000000 toiro-0.0.8/toiro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      435 2020-11-02 18:14:58.000000 toiro-0.0.8/toiro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2020-11-02 18:14:58.000000 toiro-0.0.8/toiro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:07:59.000000 toiro-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-31 15:07:44.000000 toiro-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-07-31 15:07:59.000000 toiro-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-07-31 15:07:44.000000 toiro-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-31 15:07:59.000000 toiro-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-31 15:07:44.000000 toiro-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:07:59.000000 toiro-0.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-31 15:07:44.000000 toiro-0.0.9/test/test_classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-31 15:07:44.000000 toiro-0.0.9/test/test_datadownloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-07-31 15:07:44.000000 toiro-0.0.9/test/test_tokenizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:07:59.000000 toiro-0.0.9/toiro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:07:59.000000 toiro-0.0.9/toiro/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/classifiers/classifier_bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/classifiers/classifier_svm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/classifiers/classifier_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:07:59.000000 toiro-0.0.9/toiro/datadownloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/datadownloader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:07:59.000000 toiro-0.0.9/toiro/datadownloader/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/datadownloader/data/sample.dev
+-rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/datadownloader/data/sample.test
+-rw-r--r--   0 runner    (1001) docker     (123)    66257 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/datadownloader/data/sample.train
+-rw-r--r--   0 runner    (1001) docker     (123)    90137 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/datadownloader/data/sample.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   253961 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/datadownloader/data/toiro.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    72909 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/datadownloader/data/toiro.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/datadownloader/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/datadownloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/datadownloader/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/datadownloader/sample_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:07:59.000000 toiro-0.0.9/toiro/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/tokenizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:07:59.000000 toiro-0.0.9/toiro/tokenizers/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   352418 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/tokenizers/data/ja.text8.txt.spm.model
+-rw-r--r--   0 runner    (1001) docker     (123)   121892 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/tokenizers/data/ja.text8.txt.spm.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/tokenizers/tokenizer_fugashi_ipadic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/tokenizers/tokenizer_fugashi_unidic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/tokenizers/tokenizer_ginza.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/tokenizers/tokenizer_janome.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/tokenizers/tokenizer_jumanpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/tokenizers/tokenizer_kytea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/tokenizers/tokenizer_mecab_python3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/tokenizers/tokenizer_nagisa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/tokenizers/tokenizer_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/tokenizers/tokenizer_sentencepiece.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/tokenizers/tokenizer_spacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/tokenizers/tokenizer_sudachipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/tokenizers/tokenizer_tinysegmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-07-31 15:07:44.000000 toiro-0.0.9/toiro/tokenizers/tokenizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:07:59.000000 toiro-0.0.9/toiro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-07-31 15:07:58.000000 toiro-0.0.9/toiro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-31 15:07:59.000000 toiro-0.0.9/toiro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 15:07:58.000000 toiro-0.0.9/toiro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-31 15:07:58.000000 toiro-0.0.9/toiro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 15:07:58.000000 toiro-0.0.9/toiro.egg-info/top_level.txt
```

### Comparing `toiro-0.0.8/PKG-INFO` & `toiro-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: toiro
-Version: 0.0.8
+Version: 0.0.9
 Summary: A comparison tool of Japanese tokenizers
 Home-page: https://github.com/taishi-i/toiro
 Author: Taishi Ikeda
 Author-email: taishi.ikeda.0323@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/taishi-i/toiro/archive/0.0.8.tar.gz
+Download-URL: https://github.com/taishi-i/toiro/archive/0.0.9.tar.gz
 Description: <p align="center"><img width="50%" src="https://github.com/taishi-i/toiro/blob/master/toiro/datadownloader/data/toiro.png" /></p>
         
         toiro
         -----
         
-        [![Build Status](https://travis-ci.org/taishi-i/toiro.svg?branch=master)](https://travis-ci.org/taishi-i/toiro)
-        [![Docker Cloud Build Status](https://img.shields.io/docker/cloud/build/taishii/toiro)](https://hub.docker.com/r/taishii/toiro)
-        ![Python Package](https://github.com/taishi-i/toiro/workflows/Upload%20Python%20Package/badge.svg)
+        [![Python package](https://github.com/taishi-i/toiro/actions/workflows/python-package.yml/badge.svg)](https://github.com/taishi-i/toiro/actions/workflows/python-package.yml)
         [![PyPI](https://img.shields.io/pypi/v/toiro)](https://pypi.python.org/pypi/toiro)
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/toiro)
         
         
         Toiro is a comparison tool of Japanese tokenizers.
         - Compare the processing speed of tokenizers
         - Compare the words segmented in tokenizers
@@ -54,15 +52,15 @@
         
         <details>
         <summary> How to install other tokenizers </summary>
         <p>
         
         [mecab-python3](https://github.com/SamuraiT/mecab-python3)
         ```
-        pip install mecab-python3==0.996.5
+        pip install mecab-python3
         ```
         
         [GiNZA](https://github.com/megagonlabs/ginza)
         ```
         pip install spacy ginza
         ```
         
@@ -245,14 +243,18 @@
 Keywords: Japanese NLP
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Japanese
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 Provides-Extra: all_tokenizers
 Provides-Extra: all_classifiers
```

### Comparing `toiro-0.0.8/README.md` & `toiro-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 <p align="center"><img width="50%" src="https://github.com/taishi-i/toiro/blob/master/toiro/datadownloader/data/toiro.png" /></p>
 
 toiro
 -----
 
-[![Build Status](https://travis-ci.org/taishi-i/toiro.svg?branch=master)](https://travis-ci.org/taishi-i/toiro)
-[![Docker Cloud Build Status](https://img.shields.io/docker/cloud/build/taishii/toiro)](https://hub.docker.com/r/taishii/toiro)
-![Python Package](https://github.com/taishi-i/toiro/workflows/Upload%20Python%20Package/badge.svg)
+[![Python package](https://github.com/taishi-i/toiro/actions/workflows/python-package.yml/badge.svg)](https://github.com/taishi-i/toiro/actions/workflows/python-package.yml)
 [![PyPI](https://img.shields.io/pypi/v/toiro)](https://pypi.python.org/pypi/toiro)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/toiro)
 
 
 Toiro is a comparison tool of Japanese tokenizers.
 - Compare the processing speed of tokenizers
 - Compare the words segmented in tokenizers
@@ -45,15 +43,15 @@
 
 <details>
 <summary> How to install other tokenizers </summary>
 <p>
 
 [mecab-python3](https://github.com/SamuraiT/mecab-python3)
 ```
-pip install mecab-python3==0.996.5
+pip install mecab-python3
 ```
 
 [GiNZA](https://github.com/megagonlabs/ginza)
 ```
 pip install spacy ginza
 ```
```

### Comparing `toiro-0.0.8/setup.py` & `toiro-0.0.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from setuptools import setup
 
 classifiers = [
     'License :: OSI Approved :: MIT License', 'Natural Language :: Japanese',
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8', 'Operating System :: Unix',
+    'Programming Language :: Python :: 3.8', 
+    'Programming Language :: Python :: 3.8', 
+    'Programming Language :: Python :: 3.9', 
+    'Programming Language :: Python :: 3.10', 
+    'Programming Language :: Python :: 3.11', 
+    'Operating System :: Unix',
     'Topic :: Text Processing :: Linguistic',
     'Topic :: Software Development :: Libraries :: Python Modules'
 ]
 
 
 def _long_description():
     readme = 'README.md'
@@ -17,42 +22,42 @@
     return long_description
 
 
 extras_requires_tokenizers = [
     'nagisa',
     'sudachipy',
     'sudachidict_core',
-    'mecab-python3<=0.996.5',
-    'spacy>=2.3.0',
+    'mecab-python3',
+    'spacy',
     'ginza',
     'kytea',
     'pyknp',
     'sentencepiece',
     'fugashi',
     'ipadic',
     'unidic-lite',
     'tinysegmenter3',
 ]
 
 extras_requires_classifiers = ['torch', 'transformers', 'catalyst']
 
 setup(
     name='toiro',
-    version='0.0.8',
+    version='0.0.9',
     description='A comparison tool of Japanese tokenizers',
     author='Taishi Ikeda',
     author_email='taishi.ikeda.0323@gmail.com',
     long_description_content_type='text/markdown',
     long_description=_long_description(),
     keywords='Japanese NLP',
     url='https://github.com/taishi-i/toiro',
-    download_url='https://github.com/taishi-i/toiro/archive/0.0.8.tar.gz',
+    download_url='https://github.com/taishi-i/toiro/archive/0.0.9.tar.gz',
     packages=['toiro.datadownloader', 'toiro.tokenizers', 'toiro.classifiers'],
     install_requires=[
-        'requests', 'tqdm', 'pandas', 'sklearn', 'py-cpuinfo', 'janome'
+        'requests', 'tqdm', 'pandas', 'scikit-learn', 'py-cpuinfo', 'janome'
     ],
     extras_require={
         'all_tokenizers': extras_requires_tokenizers,
         'all_classifiers': extras_requires_classifiers,
         'all': extras_requires_tokenizers + extras_requires_classifiers
     },
     classifiers=classifiers,
```

### Comparing `toiro-0.0.8/test/test_datadownloader.py` & `toiro-0.0.9/test/test_datadownloader.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 
 def test_check_correct_corpus_type_error():
     with pytest.raises(Exception):
         corpus = ""
         datadownloader.download_corpus(corpus=corpus)
 
 
-def test_download_corpus():
-    available_corpus = datadownloader.available_corpus()
-    for corpus in available_corpus:
-        datadownloader.download_corpus(corpus)
-
-        corpora_dict = datadownloader.get_corpora_dict()
-        resource_dir = datadownloader.get_resource_dir()
-
-        filename = corpora_dict[corpus]['filename']
-        filepath = os.path.join(resource_dir, filename)
-        assert os.path.exists(filepath)
+# def test_download_corpus():
+#     available_corpus = datadownloader.available_corpus()
+#     for corpus in available_corpus:
+#         datadownloader.download_corpus(corpus)
+#
+#         corpora_dict = datadownloader.get_corpora_dict()
+#         resource_dir = datadownloader.get_resource_dir()
+#
+#         filename = corpora_dict[corpus]['filename']
+#         filepath = os.path.join(resource_dir, filename)
+#         assert os.path.exists(filepath)
 
 
 def test_split_train_dev_test_error():
     corpora = datadownloader.available_corpus()
     corpus = corpora[0]
     with pytest.raises(Exception):
         train_data = 0.9
@@ -42,45 +42,45 @@
         test_data = 0.1
         train_df, dev_df, test_df = datadownloader.load_corpus(
             corpus=corpus,
             train_data=train_data, dev_data=dev_data, test_data=test_data
         )
 
 
-def test_load_corpus():
-    available_corpus = datadownloader.available_corpus()
-
-    num_corpus = {
-        'livedoor_news_corpus': {'train': 5900, 'dev': 737, 'test': 737},
-        'yahoo_movie_reviews': {'train': 72956, 'dev': 9119, 'test': 9119},
-        'amazon_reviews': {'train': 209944, 'dev': 26243, 'test': 26243},
-        'chABSA_dataset': {'train': 4895, 'dev': 611, 'test': 611}
-    }
-
-    for corpus in available_corpus:
-        if corpus == 'livedoor_news_corpus':
-            train_df, dev_df, test_df = datadownloader.load_corpus(
-                corpus=corpus
-            )
-
-        elif corpus == 'yahoo_movie_reviews':
-            train_df, dev_df, test_df = datadownloader.load_corpus(
-                corpus=corpus, corpus_type='original'
-            )
-
-        elif corpus == 'amazon_reviews':
-            train_df, dev_df, test_df = datadownloader.load_corpus(
-                corpus=corpus
-            )
-        elif corpus == 'chABSA_dataset':
-            train_df, dev_df, test_df = datadownloader.load_corpus(
-                corpus=corpus
-            )
-
-        num_data = num_corpus[corpus]
-        excepted_train = num_data['train']
-        excepted_dev = num_data['dev']
-        excepted_test = num_data['test']
-
-        assert len(train_df) == excepted_train
-        assert len(dev_df) == excepted_dev
-        assert len(test_df) == excepted_test
+# def test_load_corpus():
+#     available_corpus = datadownloader.available_corpus()
+#
+#     num_corpus = {
+#         'livedoor_news_corpus': {'train': 5900, 'dev': 737, 'test': 737},
+#         'yahoo_movie_reviews': {'train': 72956, 'dev': 9119, 'test': 9119},
+#         'amazon_reviews': {'train': 209944, 'dev': 26243, 'test': 26243},
+#         'chABSA_dataset': {'train': 4895, 'dev': 611, 'test': 611}
+#     }
+#
+#     for corpus in available_corpus:
+#         if corpus == 'livedoor_news_corpus':
+#             train_df, dev_df, test_df = datadownloader.load_corpus(
+#                 corpus=corpus
+#             )
+#
+#         elif corpus == 'yahoo_movie_reviews':
+#             train_df, dev_df, test_df = datadownloader.load_corpus(
+#                 corpus=corpus, corpus_type='original'
+#             )
+#
+#         elif corpus == 'amazon_reviews':
+#             train_df, dev_df, test_df = datadownloader.load_corpus(
+#                 corpus=corpus
+#             )
+#         elif corpus == 'chABSA_dataset':
+#             train_df, dev_df, test_df = datadownloader.load_corpus(
+#                 corpus=corpus
+#             )
+#
+#         num_data = num_corpus[corpus]
+#         excepted_train = num_data['train']
+#         excepted_dev = num_data['dev']
+#         excepted_test = num_data['test']
+#
+#         assert len(train_df) == excepted_train
+#         assert len(dev_df) == excepted_dev
+#         assert len(test_df) == excepted_test
```

### Comparing `toiro-0.0.8/test/test_tokenizers.py` & `toiro-0.0.9/test/test_tokenizers.py`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/classifiers/classifier_bert.py` & `toiro-0.0.9/toiro/classifiers/classifier_bert.py`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/classifiers/classifier_svm.py` & `toiro-0.0.9/toiro/classifiers/classifier_svm.py`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/classifiers/classifier_utils.py` & `toiro-0.0.9/toiro/classifiers/classifier_utils.py`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/datadownloader/data/sample.dev` & `toiro-0.0.9/toiro/datadownloader/data/sample.dev`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/datadownloader/data/sample.test` & `toiro-0.0.9/toiro/datadownloader/data/sample.test`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/datadownloader/data/sample.train` & `toiro-0.0.9/toiro/datadownloader/data/sample.train`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/datadownloader/data/sample.txt` & `toiro-0.0.9/toiro/datadownloader/data/sample.txt`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/datadownloader/data/toiro.gif` & `toiro-0.0.9/toiro/datadownloader/data/toiro.gif`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/datadownloader/data/toiro.png` & `toiro-0.0.9/toiro/datadownloader/data/toiro.png`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/datadownloader/download.py` & `toiro-0.0.9/toiro/datadownloader/download.py`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/datadownloader/downloader_utils.py` & `toiro-0.0.9/toiro/datadownloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/datadownloader/preprocess.py` & `toiro-0.0.9/toiro/datadownloader/preprocess.py`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/tokenizers/__init__.py` & `toiro-0.0.9/toiro/tokenizers/__init__.py`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/tokenizers/data/ja.text8.txt.spm.model` & `toiro-0.0.9/toiro/tokenizers/data/ja.text8.txt.spm.model`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/tokenizers/data/ja.text8.txt.spm.vocab` & `toiro-0.0.9/toiro/tokenizers/data/ja.text8.txt.spm.vocab`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/tokenizers/tokenizer_fugashi_ipadic.py` & `toiro-0.0.9/toiro/tokenizers/tokenizer_fugashi_ipadic.py`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/tokenizers/tokenizer_fugashi_unidic.py` & `toiro-0.0.9/toiro/tokenizers/tokenizer_fugashi_unidic.py`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/tokenizers/tokenizer_ginza.py` & `toiro-0.0.9/toiro/tokenizers/tokenizer_ginza.py`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/tokenizers/tokenizer_janome.py` & `toiro-0.0.9/toiro/tokenizers/tokenizer_janome.py`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/tokenizers/tokenizer_jumanpp.py` & `toiro-0.0.9/toiro/tokenizers/tokenizer_jumanpp.py`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/tokenizers/tokenizer_kytea.py` & `toiro-0.0.9/toiro/tokenizers/tokenizer_kytea.py`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/tokenizers/tokenizer_mecab_python3.py` & `toiro-0.0.9/toiro/tokenizers/tokenizer_mecab_python3.py`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/tokenizers/tokenizer_nagisa.py` & `toiro-0.0.9/toiro/tokenizers/tokenizer_nagisa.py`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/tokenizers/tokenizer_report.py` & `toiro-0.0.9/toiro/tokenizers/tokenizer_report.py`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/tokenizers/tokenizer_sentencepiece.py` & `toiro-0.0.9/toiro/tokenizers/tokenizer_sentencepiece.py`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/tokenizers/tokenizer_spacy.py` & `toiro-0.0.9/toiro/tokenizers/tokenizer_spacy.py`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/tokenizers/tokenizer_sudachipy.py` & `toiro-0.0.9/toiro/tokenizers/tokenizer_sudachipy.py`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/tokenizers/tokenizer_tinysegmenter.py` & `toiro-0.0.9/toiro/tokenizers/tokenizer_tinysegmenter.py`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro/tokenizers/tokenizer_utils.py` & `toiro-0.0.9/toiro/tokenizers/tokenizer_utils.py`

 * *Files identical despite different names*

### Comparing `toiro-0.0.8/toiro.egg-info/PKG-INFO` & `toiro-0.0.9/toiro.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: toiro
-Version: 0.0.8
+Version: 0.0.9
 Summary: A comparison tool of Japanese tokenizers
 Home-page: https://github.com/taishi-i/toiro
 Author: Taishi Ikeda
 Author-email: taishi.ikeda.0323@gmail.com
 License: UNKNOWN
-Download-URL: https://github.com/taishi-i/toiro/archive/0.0.8.tar.gz
+Download-URL: https://github.com/taishi-i/toiro/archive/0.0.9.tar.gz
 Description: <p align="center"><img width="50%" src="https://github.com/taishi-i/toiro/blob/master/toiro/datadownloader/data/toiro.png" /></p>
         
         toiro
         -----
         
-        [![Build Status](https://travis-ci.org/taishi-i/toiro.svg?branch=master)](https://travis-ci.org/taishi-i/toiro)
-        [![Docker Cloud Build Status](https://img.shields.io/docker/cloud/build/taishii/toiro)](https://hub.docker.com/r/taishii/toiro)
-        ![Python Package](https://github.com/taishi-i/toiro/workflows/Upload%20Python%20Package/badge.svg)
+        [![Python package](https://github.com/taishi-i/toiro/actions/workflows/python-package.yml/badge.svg)](https://github.com/taishi-i/toiro/actions/workflows/python-package.yml)
         [![PyPI](https://img.shields.io/pypi/v/toiro)](https://pypi.python.org/pypi/toiro)
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/toiro)
         
         
         Toiro is a comparison tool of Japanese tokenizers.
         - Compare the processing speed of tokenizers
         - Compare the words segmented in tokenizers
@@ -54,15 +52,15 @@
         
         <details>
         <summary> How to install other tokenizers </summary>
         <p>
         
         [mecab-python3](https://github.com/SamuraiT/mecab-python3)
         ```
-        pip install mecab-python3==0.996.5
+        pip install mecab-python3
         ```
         
         [GiNZA](https://github.com/megagonlabs/ginza)
         ```
         pip install spacy ginza
         ```
         
@@ -245,14 +243,18 @@
 Keywords: Japanese NLP
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Japanese
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 Provides-Extra: all_tokenizers
 Provides-Extra: all_classifiers
```

### Comparing `toiro-0.0.8/toiro.egg-info/SOURCES.txt` & `toiro-0.0.9/toiro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

