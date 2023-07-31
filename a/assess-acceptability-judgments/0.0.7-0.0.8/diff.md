# Comparing `tmp/assess_acceptability_judgments-0.0.7.tar.gz` & `tmp/assess_acceptability_judgments-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assess_acceptability_judgments-0.0.7.tar", last modified: Fri Jul 14 16:09:52 2023, max compression
+gzip compressed data, was "assess_acceptability_judgments-0.0.8.tar", last modified: Mon Jul 31 21:42:09 2023, max compression
```

## Comparing `assess_acceptability_judgments-0.0.7.tar` & `assess_acceptability_judgments-0.0.8.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:09:52.132751 assess_acceptability_judgments-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-14 16:09:52.136751 assess_acceptability_judgments-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:09:52.116750 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/fluency_score_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/glue.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/link_grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/nce.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/ppl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:09:52.116750 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:09:52.120750 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/nce_scores_distribution/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/nce_scores_distribution/treebank.json
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace.json
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace_llm_bert_base_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace_llm_bert_large_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace_llm_roberta_base.json
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/nce_scores_distribution/wordpiece_bert_base_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/nce_scores_distribution/wordpiece_bert_large_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/nce_scores_distribution/wordpiece_roberta_base.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:09:52.120750 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/slor_scores_distribution/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/slor_scores_distribution/treebank.json
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace.json
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace_llm_bert_base_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace_llm_bert_large_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace_llm_roberta_base.json
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/slor_scores_distribution/wordpiece_bert_base_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/slor_scores_distribution/wordpiece_bert_large_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/slor_scores_distribution/wordpiece_roberta_base.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:09:52.132751 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/words_probability/
--rw-r--r--   0 runner    (1001) docker     (123)  4196866 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/words_probability/treebank.json
--rw-r--r--   0 runner    (1001) docker     (123)  4236193 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/words_probability/whitespace.json
--rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_base_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_large_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)   885888 2023-07-14 16:09:33.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/words_probability/whitespace_llm_roberta_base.json
--rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-14 16:09:34.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_base_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-14 16:09:34.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_large_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)   917643 2023-07-14 16:09:34.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/words_probability/wordpiece_roberta_base.json
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-07-14 16:09:34.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/slor.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 16:09:50.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:09:52.116750 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-14 16:09:51.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-14 16:09:52.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:09:51.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-14 16:09:51.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-14 16:09:51.000000 assess_acceptability_judgments-0.0.7/assess_acceptability_judgments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-14 16:09:34.000000 assess_acceptability_judgments-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 16:09:52.136751 assess_acceptability_judgments-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-07-14 16:09:34.000000 assess_acceptability_judgments-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:42:09.568709 assess_acceptability_judgments-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-31 21:42:09.568709 assess_acceptability_judgments-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:42:09.552708 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/constituency_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/dependency_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/fluency_score_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/nce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/ppl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:42:09.548707 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:42:09.552708 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/nce_scores_distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/nce_scores_distribution/treebank.json
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace_llm_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace_llm_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace_llm_roberta_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/nce_scores_distribution/wordpiece_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/nce_scores_distribution/wordpiece_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/nce_scores_distribution/wordpiece_roberta_base.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:42:09.552708 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/slor_scores_distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/slor_scores_distribution/treebank.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace_llm_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace_llm_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace_llm_roberta_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/slor_scores_distribution/wordpiece_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/slor_scores_distribution/wordpiece_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/slor_scores_distribution/wordpiece_roberta_base.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:42:09.568709 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/
+-rw-r--r--   0 runner    (1001) docker     (123)  4196866 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/treebank.json
+-rw-r--r--   0 runner    (1001) docker     (123)  4236193 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/whitespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)   885888 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/whitespace_llm_roberta_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)   917643 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/wordpiece_roberta_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/slor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 21:42:09.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:42:09.552708 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-31 21:42:09.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-31 21:42:09.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 21:42:09.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-31 21:42:09.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-31 21:42:09.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-31 21:42:09.572709 assess_acceptability_judgments-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/setup.py
```

### Comparing `assess_acceptability_judgments-0.0.7/LICENSE` & `assess_acceptability_judgments-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.7/PKG-INFO` & `assess_acceptability_judgments-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: assess_acceptability_judgments
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library for assessing acceptability judgments
 Home-page: https://github.com/davebulaval/assess_acceptability_judgments
-Download-URL: https://github.com/GRAAL-Research/assess_acceptability_judgments/archive/v0.0.7.zip
+Download-URL: https://github.com/GRAAL-Research/assess_acceptability_judgments/archive/v0.0.8.zip
 Author: David Beauchemin
 Author-email: david.beauchemin.5@ulaval.ca
 License: LGPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/fluency_score_interface.py` & `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/fluency_score_interface.py`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/nce.py` & `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/nce.py`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/ppl.py` & `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/ppl.py`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/words_probability/treebank.json` & `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/treebank.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/words_probability/whitespace.json` & `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/whitespace.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_base_uncased.json` & `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_base_uncased.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_large_uncased.json` & `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_large_uncased.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/words_probability/whitespace_llm_roberta_base.json` & `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/whitespace_llm_roberta_base.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_base_uncased.json` & `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_base_uncased.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_large_uncased.json` & `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_large_uncased.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/resources/words_probability/wordpiece_roberta_base.json` & `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/wordpiece_roberta_base.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.7/assess_acceptability_judgments/slor.py` & `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/slor.py`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.7/assess_acceptability_judgments.egg-info/PKG-INFO` & `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: assess-acceptability-judgments
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library for assessing acceptability judgments
 Home-page: https://github.com/davebulaval/assess_acceptability_judgments
-Download-URL: https://github.com/GRAAL-Research/assess_acceptability_judgments/archive/v0.0.7.zip
+Download-URL: https://github.com/GRAAL-Research/assess_acceptability_judgments/archive/v0.0.8.zip
 Author: David Beauchemin
 Author-email: david.beauchemin.5@ulaval.ca
 License: LGPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `assess_acceptability_judgments-0.0.7/assess_acceptability_judgments.egg-info/SOURCES.txt` & `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 assess_acceptability_judgments/__init__.py
+assess_acceptability_judgments/constituency_parser.py
+assess_acceptability_judgments/dependency_parser.py
 assess_acceptability_judgments/fluency_score_interface.py
 assess_acceptability_judgments/glue.py
-assess_acceptability_judgments/link_grammar.py
 assess_acceptability_judgments/nce.py
 assess_acceptability_judgments/ppl.py
 assess_acceptability_judgments/slor.py
+assess_acceptability_judgments/util.py
 assess_acceptability_judgments/version.py
 assess_acceptability_judgments.egg-info/PKG-INFO
 assess_acceptability_judgments.egg-info/SOURCES.txt
 assess_acceptability_judgments.egg-info/dependency_links.txt
 assess_acceptability_judgments.egg-info/requires.txt
 assess_acceptability_judgments.egg-info/top_level.txt
 assess_acceptability_judgments/resources/nce_scores_distribution/treebank.json
```

### Comparing `assess_acceptability_judgments-0.0.7/setup.py` & `assess_acceptability_judgments-0.0.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,14 +76,21 @@
         ],
         include_package_data=True,
         install_requires=[
             "transformers",
             "torch",
             "numpy",
             "nltk",
+            "stanza",
+            "supar",
+            "benepar",
+            "spacy",
+            "spacy-transformers",
+            "progressbar",
+            "conllu",
         ],
         python_requires=">=3.8",
         description="A library for assessing acceptability judgments",
         long_description=readme,
         long_description_content_type="text/markdown",
     )
```

