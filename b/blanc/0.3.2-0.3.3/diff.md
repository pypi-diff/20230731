# Comparing `tmp/blanc-0.3.2.tar.gz` & `tmp/blanc-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blanc-0.3.2.tar", last modified: Tue Jul 25 15:58:14 2023, max compression
+gzip compressed data, was "blanc-0.3.3.tar", last modified: Mon Jul 31 15:34:03 2023, max compression
```

## Comparing `blanc-0.3.2.tar` & `blanc-0.3.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-25 15:58:14.173191 blanc-0.3.2/
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-25 15:58:14.156981 blanc-0.3.2/.github/
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-25 15:58:14.158835 blanc-0.3.2/.github/workflows/
--rw-r--r--   0 olegvasilyev   (502) staff       (20)     2532 2022-11-20 20:03:24.000000 blanc-0.3.2/.github/workflows/codeql-analysis.yml
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)       54 2020-04-22 21:28:28.000000 blanc-0.3.2/.gitignore
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)     1049 2020-04-22 21:28:28.000000 blanc-0.3.2/LICENSE
--rw-r--r--   0 olegvasilyev   (502) staff       (20)    13913 2023-07-25 15:58:14.172984 blanc-0.3.2/PKG-INFO
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)    13478 2022-02-10 23:08:14.000000 blanc-0.3.2/README.md
--rw-r--r--   0 olegvasilyev   (502) staff       (20)     1629 2022-11-20 20:03:24.000000 blanc-0.3.2/SECURITY.md
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-25 15:58:14.160749 blanc-0.3.2/blanc/
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)      133 2022-02-10 23:08:14.000000 blanc-0.3.2/blanc/__init__.py
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)    12173 2021-09-01 21:24:46.000000 blanc-0.3.2/blanc/__main__.py
--rw-r--r--   0 olegvasilyev   (502) staff       (20)       22 2023-07-25 15:57:40.000000 blanc-0.3.2/blanc/__version__.py
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)    36885 2023-06-26 23:31:35.000000 blanc-0.3.2/blanc/blanc.py
--rw-r--r--   0 olegvasilyev   (502) staff       (20)    20104 2023-07-25 15:57:40.000000 blanc-0.3.2/blanc/estime.py
--rw-r--r--   0 olegvasilyev   (502) staff       (20)    11877 2023-06-26 23:53:08.000000 blanc-0.3.2/blanc/shannon.py
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)    16178 2021-03-11 01:31:26.000000 blanc-0.3.2/blanc/utils.py
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-25 15:58:14.161580 blanc-0.3.2/blanc.egg-info/
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)    13913 2023-07-25 15:58:14.000000 blanc-0.3.2/blanc.egg-info/PKG-INFO
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)      617 2023-07-25 15:58:14.000000 blanc-0.3.2/blanc.egg-info/SOURCES.txt
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)        1 2023-07-25 15:58:14.000000 blanc-0.3.2/blanc.egg-info/dependency_links.txt
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)       46 2023-07-25 15:58:14.000000 blanc-0.3.2/blanc.egg-info/entry_points.txt
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)       98 2023-07-25 15:58:14.000000 blanc-0.3.2/blanc.egg-info/requires.txt
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)        6 2023-07-25 15:58:14.000000 blanc-0.3.2/blanc.egg-info/top_level.txt
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-25 15:58:14.171839 blanc-0.3.2/data/
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)  2779006 2020-11-22 22:52:16.000000 blanc-0.3.2/data/CNN_DailyMail_555.json
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)  1110748 2020-11-22 22:52:16.000000 blanc-0.3.2/data/DailyNews_300.json
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)  1257825 2020-11-22 22:52:16.000000 blanc-0.3.2/data/DailyNews_300_aspects.json
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)     1361 2021-04-04 18:11:32.000000 blanc-0.3.2/data/README.md
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)      506 2020-04-22 21:28:28.000000 blanc-0.3.2/data/doc-summaries.json
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)      363 2020-04-22 21:28:28.000000 blanc-0.3.2/data/pairs.json
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)      149 2020-04-22 21:28:28.000000 blanc-0.3.2/data/single.json
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-25 15:58:14.171980 blanc-0.3.2/estime/
--rw-r--r--   0 olegvasilyev   (502) staff       (20)     4053 2023-06-26 23:53:08.000000 blanc-0.3.2/estime/README.md
--rw-r--r--   0 olegvasilyev   (502) staff       (20)       98 2022-11-21 01:28:17.000000 blanc-0.3.2/requirements.txt
--rw-r--r--   0 olegvasilyev   (502) staff       (20)       38 2023-07-25 15:58:14.173236 blanc-0.3.2/setup.cfg
--rw-r--r--   0 olegvasilyev   (502) staff       (20)      948 2023-07-25 15:57:40.000000 blanc-0.3.2/setup.py
-drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-25 15:58:14.172545 blanc-0.3.2/shannon/
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)      419 2022-11-27 18:48:19.000000 blanc-0.3.2/shannon/README.md
--rw-rw-r--   0 olegvasilyev   (502) staff       (20)     3541 2022-02-01 01:02:52.000000 blanc-0.3.2/shannon/summeval_score.py
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-31 15:34:03.406234 blanc-0.3.3/
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-31 15:34:03.391523 blanc-0.3.3/.github/
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-31 15:34:03.393151 blanc-0.3.3/.github/workflows/
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)     2532 2022-11-20 20:03:24.000000 blanc-0.3.3/.github/workflows/codeql-analysis.yml
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)       54 2020-04-22 21:28:28.000000 blanc-0.3.3/.gitignore
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)     1049 2020-04-22 21:28:28.000000 blanc-0.3.3/LICENSE
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)    13913 2023-07-31 15:34:03.406072 blanc-0.3.3/PKG-INFO
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)    13478 2022-02-10 23:08:14.000000 blanc-0.3.3/README.md
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)     1629 2022-11-20 20:03:24.000000 blanc-0.3.3/SECURITY.md
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-31 15:34:03.394986 blanc-0.3.3/blanc/
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)      133 2022-02-10 23:08:14.000000 blanc-0.3.3/blanc/__init__.py
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)    12173 2021-09-01 21:24:46.000000 blanc-0.3.3/blanc/__main__.py
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)       22 2023-07-31 15:33:41.000000 blanc-0.3.3/blanc/__version__.py
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)    36885 2023-06-26 23:31:35.000000 blanc-0.3.3/blanc/blanc.py
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)    21153 2023-07-31 15:33:41.000000 blanc-0.3.3/blanc/estime.py
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)    11877 2023-06-26 23:53:08.000000 blanc-0.3.3/blanc/shannon.py
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)    16178 2021-03-11 01:31:26.000000 blanc-0.3.3/blanc/utils.py
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-31 15:34:03.395773 blanc-0.3.3/blanc.egg-info/
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)    13913 2023-07-31 15:34:03.000000 blanc-0.3.3/blanc.egg-info/PKG-INFO
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)      617 2023-07-31 15:34:03.000000 blanc-0.3.3/blanc.egg-info/SOURCES.txt
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)        1 2023-07-31 15:34:03.000000 blanc-0.3.3/blanc.egg-info/dependency_links.txt
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)       46 2023-07-31 15:34:03.000000 blanc-0.3.3/blanc.egg-info/entry_points.txt
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)       98 2023-07-31 15:34:03.000000 blanc-0.3.3/blanc.egg-info/requires.txt
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)        6 2023-07-31 15:34:03.000000 blanc-0.3.3/blanc.egg-info/top_level.txt
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-31 15:34:03.403076 blanc-0.3.3/data/
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)  2779006 2020-11-22 22:52:16.000000 blanc-0.3.3/data/CNN_DailyMail_555.json
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)  1110748 2020-11-22 22:52:16.000000 blanc-0.3.3/data/DailyNews_300.json
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)  1257825 2020-11-22 22:52:16.000000 blanc-0.3.3/data/DailyNews_300_aspects.json
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)     1361 2021-04-04 18:11:32.000000 blanc-0.3.3/data/README.md
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)      506 2020-04-22 21:28:28.000000 blanc-0.3.3/data/doc-summaries.json
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)      363 2020-04-22 21:28:28.000000 blanc-0.3.3/data/pairs.json
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)      149 2020-04-22 21:28:28.000000 blanc-0.3.3/data/single.json
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-31 15:34:03.403230 blanc-0.3.3/estime/
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)     5279 2023-07-31 15:33:41.000000 blanc-0.3.3/estime/README.md
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)       98 2022-11-21 01:28:17.000000 blanc-0.3.3/requirements.txt
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)       38 2023-07-31 15:34:03.406281 blanc-0.3.3/setup.cfg
+-rw-r--r--   0 olegvasilyev   (502) staff       (20)      948 2023-07-31 15:33:41.000000 blanc-0.3.3/setup.py
+drwxr-xr-x   0 olegvasilyev   (502) staff       (20)        0 2023-07-31 15:34:03.405717 blanc-0.3.3/shannon/
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)      419 2022-11-27 18:48:19.000000 blanc-0.3.3/shannon/README.md
+-rw-rw-r--   0 olegvasilyev   (502) staff       (20)     3541 2022-02-01 01:02:52.000000 blanc-0.3.3/shannon/summeval_score.py
```

### Comparing `blanc-0.3.2/.github/workflows/codeql-analysis.yml` & `blanc-0.3.3/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `blanc-0.3.2/LICENSE` & `blanc-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `blanc-0.3.2/PKG-INFO` & `blanc-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blanc
-Version: 0.3.2
+Version: 0.3.3
 Summary: Human-free quality estimation of document summaries
 Home-page: https://github.com/PrimerAI/blanc
 Author: Primer AI
 Author-email: blanc@primer.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `blanc-0.3.2/README.md` & `blanc-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `blanc-0.3.2/SECURITY.md` & `blanc-0.3.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `blanc-0.3.2/blanc/__main__.py` & `blanc-0.3.3/blanc/__main__.py`

 * *Files identical despite different names*

### Comparing `blanc-0.3.2/blanc/blanc.py` & `blanc-0.3.3/blanc/blanc.py`

 * *Files identical despite different names*

### Comparing `blanc-0.3.2/blanc/estime.py` & `blanc-0.3.3/blanc/estime.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,90 +12,91 @@
 
 import torch
 from transformers import BertForMaskedLM, BertTokenizer, BertModel
 
 
 class Estime:
     """Estimator of factual inconsistencies between summaries (or other textual claims)
-    and text. Usage: create `Estime`, and use `evaluate_claims`.
-    To get all the measures, use output=['alarms', 'soft', 'coherence'].
+    and text. Usage: create `Estime`, and use `evaluate_claims()`.
+    In creating Estime, specify the names of the desired measures in the list 'output'. 
+    The function evaluate_claims() will return (for each claim) the list of results in 
+    the same order. The list 'output' can also include:
+        'alarms': the original ESTIME
+        'alarms_adjusted': the original ESTIME, extrapolated to non-overlapping tokens
+        'alarms_alltokens': ESTIME on all (not only overlapped) summary tokens
+        'soft': the soft ESTIME
+        'coherence': measure of summary coherence
     """
     def __init__(
         self,
         path_mdl='bert-large-uncased-whole-word-masking',
         path_mdl_raw='bert-base-uncased',
         i_layer_context=21,
         device='cpu',
         output=['alarms'],
         tags_check=None,
         tags_exclude=None,
         input_size_max=450,
         margin=50,
-        distance_word_min=8,
-        include_all_tokens=False):
-        """
-        If output includes either 'soft' or 'coherence', then all the summary tokens are considered,
-        (regardless of 'include_all_tokens'), as it should be for 'soft' and 'coherence'. 
-        If output is only 'alarms', then all the summary tokens are considered only with the setting
-        include_all_tokens=True. The default include_all_tokens=False corresponds to the original 
-        'hard' ESTIME, and is appropriate for normal summaries that have a reasonable tokens overlap 
-        with the text. The original 'hard' ESTIME is useless for intentionally abnormal summaries that 
-        have no any tokens common with text: it would give zero alarms.  
+        distance_word_min=8):
+        """  
         Args:
             path_mdl (str): model for embeddings of masked tokens
             path_mdl_raw (str): model for raw embeddings
             i_layer_context (int): index of layer to take contextual embeddings from
             device (str): 'cpu' or 'cuda'
             tags_check (List[str]): list of parts of speech to use, each is a tag
                 by NLTK notations. If None, then all words will be used, 
                 no matter which parts of speech they are.
             tags_exclude (List[str]): List or set of part-of-speach tags that should
                 not be considered. Has priority over tags_check.
-            include_all_tokens (Boolean): If True then all summary tokens are considered.
-                If False and if output includes only 'alarms', then only tokens existing in the text are considered.
             input_size_max (int): length of input for the model as number of tokens
             margin (int): number of tokens on input edges not to take embeddings from
             distance_word_min (int): minimal distance between the masked tokens 
                 from which embeddings are to ne taken in a single input
-            output (List[str]): list of names of measures to get in claim evaluations
-
+            output (List[str]): list of names of measures to get in claim evaluations. 
+                The list must be nonempty and can include:
+                'alarms', 'alarms_adjusted', 'alarms_alltokens', 'soft', 'coherence'.
+                The function evaluate_claims() will return (for each claim) the list of 
+                results in the same order.
         """
         self.i_layer_context = i_layer_context
         self.device = device
+        assert output
         self.output = output
-        self.ESTIME_ALARMS = 'alarms'  # original estime by response of tokens to similar contexts
-        self.ESTIME_SOFT = 'soft'  # soft estime by response of cos between embeddings
-        self.ESTIME_COHERENCE = 'coherence'  # estimation of summary coherence 
+        self.ESTIME_ALARMS = 'alarms'  # original estime: by response of tokens to similar contexts
+        self.ESTIME_ALLTOKENS = 'alarms_alltokens'  # estime on all (not only overlapped) summary tokens
+        self.ESTIME_ADJUSTED = 'alarms_adjusted'  # original estime, extrapolated to non-overlapping tokens
+        self.ESTIME_SOFT = 'soft'  # soft estime by response of similarity between embeddings
+        self.ESTIME_COHERENCE = 'coherence'  # estimation of summary coherence
+        self.get_estime_adjusted = self.ESTIME_ADJUSTED in self.output
         self.get_estime_soft = self.ESTIME_SOFT in self.output
         self.get_estime_coherence = self.ESTIME_COHERENCE in self.output
         self.tags_check = tags_check
         self.tags_exclude = tags_exclude
         self.input_size_max = input_size_max
         self.margin = margin
         self.distance_word_min = distance_word_min
-        self.include_all_tokens = include_all_tokens
-        if 'soft' in output or 'coherence' in output:
-            self.include_all_tokens = True
         self.model_tokenizer = None
         self.model = None
         self.model_tokenizer = BertTokenizer.from_pretrained(path_mdl)
         self.model = BertForMaskedLM.from_pretrained(path_mdl, output_hidden_states = True).to(self.device)
         self.model.eval()
         if self.get_estime_soft:
             self.model_raw = BertModel.from_pretrained(path_mdl_raw)
             self.model_raw.eval()
             for param in self.model_raw.parameters():
                 param.requires_grad = False
             self.embeddings_raw = self.model_raw.get_input_embeddings()
-        # Convenient data (tokenized summary and text):
+        # Convenient data (including tokenized summary and text):
+        self.text_map_wordscheck = None
         self.summ_toks = None 
         self.text_toks = None
         self.embs_mask_text = None
         self.embs_raw_text = None
-        
 
 
     def evaluate_claims(self, text, claims):
         """
         Given a text, and a list of claims (e.g. summaries, or other texts), 
         estimates how many likely factual inconsistencies each claim contains
         (the inconsistencies are with respect to the text).
@@ -111,31 +112,28 @@
                 accordingly to the names in self.output.
         """
         # Text:
         text = unicodedata.normalize('NFKD', text)
         text_words = word_tokenize(text)
         text_tagged = nltk.pos_tag(text_words)
         # Find all words of interest in the text, tokenize:
-        text_map_wordscheck = self._get_map_words_intext(text_tagged)
-        text_iwordscheck = sorted([item for sublist in text_map_wordscheck.values() for item in sublist])
+        self.text_map_wordscheck = self._get_map_words_intext(text_tagged)
+        text_iwordscheck = sorted([item for sublist in self.text_map_wordscheck.values() for item in sublist])
         self.text_toks, text_map_iword_itoks = self._translate_words_to_tokens(text_words)
         # All embeddings of interest in the text:
         self.embs_mask_text = self._get_embeddings(
             tokens=self.text_toks, 
             ixs_words=text_iwordscheck, 
             map_words_to_tokens=text_map_iword_itoks)
         self.embs_raw_text = self._get_embeddings_raw(tokens=self.text_toks)
         # Get the consistency info for each claim:
         claims_info = []
         for claim in claims:
             claim = unicodedata.normalize('NFKD', claim)
-            if self.include_all_tokens:
-                claim_info = self._evaluate_claim(claim)
-            else:
-                claim_info = self._evaluate_claim(claim, text_map_wordscheck)
+            claim_info = self._evaluate_claim(claim)
             claims_info.append(claim_info)
         self.summ_toks = None 
         self.text_toks = None
         return claims_info
 
 
     def _evaluate_claim(self, claim, words_check=None):
@@ -147,27 +145,31 @@
                 of interest in the main text
         Returns:
             estime_info (List[float]): a list with results corresponding to the 
                 names of measures specified in self.output.
         """
         summ_words = word_tokenize(claim)
         summ_tagged = nltk.pos_tag(summ_words)
-        # Find all words of interest in the summary:
-        summ_iwordscheck = []
+        summ_iwordscheck, summ_iwords_overlap = [],[]  # Find all words of interest in the summary
         for i, (w, t) in enumerate(summ_tagged):
             if not words_check or w in words_check:  # if required, checking only what exists in the text
                 summ_iwordscheck.append(i)
+            if not self.text_map_wordscheck or w in self.text_map_wordscheck:
+                summ_iwords_overlap.append(i)
         self.summ_toks, summ_map_iword_itoks = self._translate_words_to_tokens(summ_words)
         embs_mask_summ = self._get_embeddings(
             tokens=self.summ_toks, ixs_words=summ_iwordscheck, map_words_to_tokens=summ_map_iword_itoks)
         embs_raw_summ = self._get_embeddings_raw(tokens=self.summ_toks)
-        # Consider only some layers:
+        summ_itoksoverlap = set()
+        for iword in summ_iwords_overlap:
+            itok = summ_map_iword_itoks[iword][0]  # only first token of each word
+            summ_itoksoverlap.add(itok)
         estime_info = self._evaluate(
             embs_mask_summ, self.embs_mask_text, 
-            embs_raw_summ, self.embs_raw_text)
+            embs_raw_summ, self.embs_raw_text, summ_itokscheck=summ_itoksoverlap)
         return estime_info
 
 
     def _get_embeddings_raw(self, tokens):
         """Simply gets raw embeddings. Needed only for estime-soft."""
         if not self.get_estime_soft:
             return None
@@ -271,67 +273,81 @@
             for i in range(word_toks[0], word_toks[1]):
                 input_toks[i - ix_toks_input_beg] = '[MASK]'
         # Get embeddings of interest for this input:
         toks_ids = self.model_tokenizer.convert_tokens_to_ids(['[CLS]'] + input_toks + ['[SEP]'])
         input_tensor = torch.LongTensor([toks_ids]).to(self.device)
         outputs = self.model(input_tensor)
         # Contextual embedding:
-        emb_all = outputs[1][self.i_layer_context][0]  # all embeddings (means: for all tokens, at this layer)
+        emb_all = outputs[1][self.i_layer_context][0]  # all embeddings (for all tokens, at this layer)
         map_itok_embed = {}
         for itok, iembed in map_itok_iembed.items():  # itok is id of token exactly as in tokens
             map_itok_embed[itok] = emb_all[iembed].cpu().detach().numpy()
         return map_itok_embed
 
 
-    def _evaluate(self, embs_summ, embs_text, embs_summ_raw, embs_text_raw):
+    def _evaluate(self, embs_summ, embs_text, embs_summ_raw, embs_text_raw, summ_itokscheck=None):
         """
         Args:
             embs_summ (Dict{int: List[float]}): Map of token indexes 
                 (in summary) to the corresponding embeddings
             embs_text (Dict{int: List[float]}): Map of token indexes 
                 (in text) to the corresponding embeddings
-            embs_summ_raw and embs_text_raw - the same as above,
-                but with the raw embeddings
+            embs_summ_raw and embs_text_raw - the same as above, but with the raw embeddings
+            summ_itokscheck (Set[int]): Set of indexes of tokens (in summary)
+                that must be verified for alarms. 
+                This is needed for calculating the original and 'adjusted' ESTIME.
         Returns:
-            List[float)] - List of results as specified in self.output
+            List[float)] - List of results in order as specified in self.output
         """
-        # estime standard and soft:
-        n_alarms, cos_raw_avg = 0, 0
+        # estime standard, adjusted, all-tokens and soft:
+        n_alarms, n_alarms_alltoks, cos_raw_avg = 0, 0, 0
         itoks_similar = []
         for itok_summ, emb_summ in embs_summ.items():   
             tok_summ = self.summ_toks[itok_summ]
             itok_text_best = -1
             sim_best = -1.0e30
             for itok_text, emb_text in embs_text.items():
                 sim = dot(emb_summ, emb_text)
                 if sim > sim_best:
                     sim_best = sim
                     itok_text_best = itok_text
             tok_text_best = self.text_toks[itok_text_best]
             itoks_similar.append((itok_summ, itok_text_best, sim_best))
             if tok_text_best != tok_summ:
-                n_alarms += 1
+                n_alarms_alltoks += 1
+                if not summ_itokscheck or itok_summ in summ_itokscheck:
+                    n_alarms += 1
             # Soft estime:
             if self.get_estime_soft:
                 emb_summ_nomask = embs_summ_raw[itok_summ]
                 emb_text_nomask = embs_text_raw[itok_text_best]
                 prod = dot(emb_summ_nomask, emb_text_nomask)
                 norm_summ, norm_text = norm(emb_summ_nomask), norm(emb_text_nomask)
                 cos_raw_avg += prod / (norm_summ * norm_text)
         if self.get_estime_soft:
             cos_raw_avg /= len(embs_summ)
+        # estime-alarms-adjusted:
+        if self.get_estime_adjusted:
+            if not summ_itokscheck:
+                n_alarms_adj = len(embs_summ)
+            else:
+                n_alarms_adj = n_alarms * len(embs_summ) / len(summ_itokscheck)
         # Coherence:
         if self.get_estime_coherence:
             itoks_summ = [a[0] for a in itoks_similar]
             itoks_text = [a[1] for a in itoks_similar]
             coherence = scipy.stats.kendalltau(itoks_summ, itoks_text, variant='c').correlation
         result = []
         for out_name in self.output:
             if out_name == self.ESTIME_ALARMS:
                 result.append(n_alarms)
+            elif out_name == self.ESTIME_ADJUSTED:
+                result.append(n_alarms_adj)
+            elif out_name == self.ESTIME_ALLTOKENS:
+                result.append(n_alarms_alltoks)
             elif out_name == self.ESTIME_SOFT:
                 result.append(cos_raw_avg)
             elif out_name == self.ESTIME_COHERENCE:
                 result.append(coherence)
         return result
```

### Comparing `blanc-0.3.2/blanc/shannon.py` & `blanc-0.3.3/blanc/shannon.py`

 * *Files identical despite different names*

### Comparing `blanc-0.3.2/blanc/utils.py` & `blanc-0.3.3/blanc/utils.py`

 * *Files identical despite different names*

### Comparing `blanc-0.3.2/blanc.egg-info/PKG-INFO` & `blanc-0.3.3/blanc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blanc
-Version: 0.3.2
+Version: 0.3.3
 Summary: Human-free quality estimation of document summaries
 Home-page: https://github.com/PrimerAI/blanc
 Author: Primer AI
 Author-email: blanc@primer.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `blanc-0.3.2/blanc.egg-info/SOURCES.txt` & `blanc-0.3.3/blanc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blanc-0.3.2/data/CNN_DailyMail_555.json` & `blanc-0.3.3/data/CNN_DailyMail_555.json`

 * *Files identical despite different names*

### Comparing `blanc-0.3.2/data/DailyNews_300.json` & `blanc-0.3.3/data/DailyNews_300.json`

 * *Files identical despite different names*

### Comparing `blanc-0.3.2/data/DailyNews_300_aspects.json` & `blanc-0.3.3/data/DailyNews_300_aspects.json`

 * *Files identical despite different names*

### Comparing `blanc-0.3.2/data/README.md` & `blanc-0.3.3/data/README.md`

 * *Files identical despite different names*

### Comparing `blanc-0.3.2/estime/README.md` & `blanc-0.3.3/estime/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -12,21 +12,24 @@
 >>> estimator = Estime()
 >>> text = """In Kander’s telling, Mandel called him up out of the blue a decade or so ago to pitch a project. It made sense why. The two men had similar profiles: Jewish combat veterans in their early 30s. New statewide officeholders in the Midwest."""
 >>> summary = """Kander and Mandel had similar profiles, and it makes sense."""
 >>> estimator.evaluate_claims(text, [summary])
 [[5]]
 ```
 
-In this example only one summary is given to the text, and hence the list of results contains only one element [5] - the scores only for this summary. The scores list contains only single score =5, because by default the list of measures contains only one measure 'alarms'. More measures can be included, e.g.: 
+Default `device` in Estime() is `device`='cpu'. It can be set `device`='cuda'.
+
+In the example above only one summary is given to the text, and hence the list of results contains only one element [5] - the scores only for this summary. The scores list contains only single score =5, because by default the list of measures contains only one measure 'alarms'. More measures can be included: 'alarms', 'alarms_adjusted', 'alarms_alltokens', 'soft', 'coherence'. For example:
 
 ```
->>> estimator = Estime(output=['alarms', 'soft', 'coherence'])
+>>> estimator = Estime(output=['alarms', 'alarms_adjusted', 'soft', 'coherence'])
 >>> estimator.evaluate_claims(text, [summary])
-[[5, 0.502, -0.25]]
+[[5, 7.5, 0.502, -0.25]]
 ```
+The results appear in the same order as the names given in `output`. The measures 'alarms' (the original ESTIME), 'soft' and 'coherence' are as defined in the papers. The only difference is that when there are no any tokens overlap between the claim and the text, the 'alarms' is set to the number of the tokens in the summary. Unlike 'soft', the original ESTIME does not make good estimation for the cases where the number of overlap tokens is much less than the total number of summary tokens. Starting from the version 0.3.3, the measure 'alarms_adjusted' can be added. It is defined as `alarms_adjusted = alarms * N / M`, where M is the number of overlap tokens, and N is the total number of summary tokens. Thus, it serves as an extrapolation of the 'alarms' to the total number of summary tokens. When M=0, the 'alarms_adjusted' is set to N. For curiocity (not recommended), the 'alarms_alltokens' also can be added, it is defined as `alarms_alltokens = alarms + N - M`, meaning that any non-overlapping token is counted as an alarm. 
 
 For more options, see comments in the source [estime](https://github.com/PrimerAI/blanc/blob/master/blanc/estime.py), or see [estime](https://github.com/PrimerAI/primer-research/tree/main/estime).
 
 The table below is made in the same way as the Table 1 in [ESTIME](https://aclanthology.org/2021.eval4nlp-1.10/), except that the number of systems here is updated from 16 to 17, following the later version of [SummEval](https://direct.mit.edu/tacl/article/doi/10.1162/tacl_a_00373/100686/SummEval-Re-evaluating-Summarization-Evaluation). This means that the correlations are taken here between arrays of 1700-length (100 texts x 17 summary generation systems).
 
 |model|consistency<br />Spearman|consistency<br />Kendall|relevance<br />Spearman|relevance<br />Kendall|coherence<br />Spearman|coherence<br />Kendall|fluency<br />Spearman|fluency<br />Kendall|
 |:--|--:|--:|--:|--:|--:|--:|--:|--:|
```

### Comparing `blanc-0.3.2/setup.py` & `blanc-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import setuptools
 
-version = "0.3.2"
+version = "0.3.3"
 
 with open("README.md", encoding="utf-8") as reader:
     long_description = reader.read()
 
 with open("requirements.txt") as reader:
     requirements = [line.strip() for line in reader]
```

### Comparing `blanc-0.3.2/shannon/summeval_score.py` & `blanc-0.3.3/shannon/summeval_score.py`

 * *Files identical despite different names*

