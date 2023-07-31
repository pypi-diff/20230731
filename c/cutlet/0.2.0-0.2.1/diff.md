# Comparing `tmp/cutlet-0.2.0.tar.gz` & `tmp/cutlet-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cutlet-0.2.0.tar", last modified: Wed Jun 14 13:16:30 2023, max compression
+gzip compressed data, was "cutlet-0.2.1.tar", last modified: Mon Jul 31 13:52:19 2023, max compression
```

## Comparing `cutlet-0.2.0.tar` & `cutlet-0.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:16:30.025344 cutlet-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:16:30.025344 cutlet-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-14 13:15:51.000000 cutlet-0.2.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:16:30.025344 cutlet-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-14 13:15:51.000000 cutlet-0.2.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-14 13:15:51.000000 cutlet-0.2.0/.github/workflows/linux.yml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-14 13:15:51.000000 cutlet-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-14 13:15:51.000000 cutlet-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-14 13:15:51.000000 cutlet-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-06-14 13:16:30.025344 cutlet-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-14 13:15:51.000000 cutlet-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:16:30.025344 cutlet-0.2.0/cutlet/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-14 13:15:51.000000 cutlet-0.2.0/cutlet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-14 13:15:51.000000 cutlet-0.2.0/cutlet/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    13243 2023-06-14 13:15:51.000000 cutlet-0.2.0/cutlet/cutlet.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-14 13:15:51.000000 cutlet-0.2.0/cutlet/exceptions.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-14 13:15:51.000000 cutlet-0.2.0/cutlet/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:16:30.025344 cutlet-0.2.0/cutlet/test/
--rw-r--r--   0 runner    (1001) docker     (123)    27191 2023-06-14 13:15:51.000000 cutlet-0.2.0/cutlet/test/blns.json
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-06-14 13:15:51.000000 cutlet-0.2.0/cutlet/test/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-14 13:15:51.000000 cutlet-0.2.0/cutlet/test/test_fuzz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:16:30.025344 cutlet-0.2.0/cutlet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-06-14 13:16:29.000000 cutlet-0.2.0/cutlet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-14 13:16:29.000000 cutlet-0.2.0/cutlet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 13:16:29.000000 cutlet-0.2.0/cutlet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-14 13:16:29.000000 cutlet-0.2.0/cutlet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-14 13:16:29.000000 cutlet-0.2.0/cutlet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 13:16:29.000000 cutlet-0.2.0/cutlet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)   340278 2023-06-14 13:15:51.000000 cutlet-0.2.0/cutlet.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:16:30.025344 cutlet-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   189912 2023-06-14 13:15:51.000000 cutlet-0.2.0/docs/cutlet.html
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-14 13:15:51.000000 cutlet-0.2.0/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    90584 2023-06-14 13:15:51.000000 cutlet-0.2.0/docs/search.js
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-14 13:15:51.000000 cutlet-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-14 13:15:51.000000 cutlet-0.2.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-14 13:15:51.000000 cutlet-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 13:16:30.025344 cutlet-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-14 13:15:51.000000 cutlet-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:52:19.941105 cutlet-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:52:19.941105 cutlet-0.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 13:51:40.000000 cutlet-0.2.1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:52:19.941105 cutlet-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-31 13:51:40.000000 cutlet-0.2.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-31 13:51:40.000000 cutlet-0.2.1/.github/workflows/linux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 13:51:40.000000 cutlet-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-31 13:51:40.000000 cutlet-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-31 13:51:40.000000 cutlet-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-07-31 13:52:19.941105 cutlet-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-31 13:51:40.000000 cutlet-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:52:19.941105 cutlet-0.2.1/cutlet/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-31 13:51:40.000000 cutlet-0.2.1/cutlet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-31 13:51:40.000000 cutlet-0.2.1/cutlet/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13237 2023-07-31 13:51:40.000000 cutlet-0.2.1/cutlet/cutlet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-31 13:51:40.000000 cutlet-0.2.1/cutlet/exceptions.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-31 13:51:40.000000 cutlet-0.2.1/cutlet/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:52:19.941105 cutlet-0.2.1/cutlet/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    27191 2023-07-31 13:51:40.000000 cutlet-0.2.1/cutlet/test/blns.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-07-31 13:51:40.000000 cutlet-0.2.1/cutlet/test/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-31 13:51:40.000000 cutlet-0.2.1/cutlet/test/test_fuzz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:52:19.941105 cutlet-0.2.1/cutlet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-07-31 13:52:19.000000 cutlet-0.2.1/cutlet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-31 13:52:19.000000 cutlet-0.2.1/cutlet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 13:52:19.000000 cutlet-0.2.1/cutlet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 13:52:19.000000 cutlet-0.2.1/cutlet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-31 13:52:19.000000 cutlet-0.2.1/cutlet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-31 13:52:19.000000 cutlet-0.2.1/cutlet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   340278 2023-07-31 13:51:40.000000 cutlet-0.2.1/cutlet.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:52:19.941105 cutlet-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   189912 2023-07-31 13:51:40.000000 cutlet-0.2.1/docs/cutlet.html
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-31 13:51:40.000000 cutlet-0.2.1/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    90584 2023-07-31 13:51:40.000000 cutlet-0.2.1/docs/search.js
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-31 13:51:40.000000 cutlet-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-31 13:51:40.000000 cutlet-0.2.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-31 13:51:40.000000 cutlet-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 13:52:19.941105 cutlet-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-31 13:51:40.000000 cutlet-0.2.1/setup.py
```

### Comparing `cutlet-0.2.0/.github/workflows/docs.yml` & `cutlet-0.2.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `cutlet-0.2.0/.github/workflows/linux.yml` & `cutlet-0.2.1/.github/workflows/linux.yml`

 * *Files identical despite different names*

### Comparing `cutlet-0.2.0/LICENSE` & `cutlet-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cutlet-0.2.0/PKG-INFO` & `cutlet-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cutlet
-Version: 0.2.0
+Version: 0.2.1
 Summary: Romaji converter
 Home-page: https://github.com/polm/cutlet
 Author: Paul O'Leary McCann
 Author-email: polm@dampfkraft.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Japanese
 Requires-Python: >=3.5
@@ -14,15 +14,15 @@
 [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://share.streamlit.io/polm/cutlet-demo/main/demo.py)
 [![Current PyPI packages](https://badge.fury.io/py/cutlet.svg)](https://pypi.org/project/cutlet/)
 
 # cutlet
 
 <img src="https://github.com/polm/cutlet/raw/master/cutlet.png" width=125 height=125 alt="cutlet by Irasutoya" />
 
-Cutlet is a tool to convert Japanese to romaji. Check out the [interactive demo][demo]!
+Cutlet is a tool to convert Japanese to romaji. Check out the [interactive demo][demo]! Also see the [docs](https://polm.github.io/cutlet/cutlet.html) and the [original blog post](https://www.dampfkraft.com/nlp/cutlet-python-romaji-converter.html). 
 
 [demo]: https://share.streamlit.io/polm/cutlet-demo/main/demo.py
 
 **issueを英語で書く必要はありません。**
 
 Features:
```

### Comparing `cutlet-0.2.0/README.md` & `cutlet-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://share.streamlit.io/polm/cutlet-demo/main/demo.py)
 [![Current PyPI packages](https://badge.fury.io/py/cutlet.svg)](https://pypi.org/project/cutlet/)
 
 # cutlet
 
 <img src="https://github.com/polm/cutlet/raw/master/cutlet.png" width=125 height=125 alt="cutlet by Irasutoya" />
 
-Cutlet is a tool to convert Japanese to romaji. Check out the [interactive demo][demo]!
+Cutlet is a tool to convert Japanese to romaji. Check out the [interactive demo][demo]! Also see the [docs](https://polm.github.io/cutlet/cutlet.html) and the [original blog post](https://www.dampfkraft.com/nlp/cutlet-python-romaji-converter.html). 
 
 [demo]: https://share.streamlit.io/polm/cutlet-demo/main/demo.py
 
 **issueを英語で書く必要はありません。**
 
 Features:
```

### Comparing `cutlet-0.2.0/cutlet/cutlet.py` & `cutlet-0.2.1/cutlet/cutlet.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,28 +22,28 @@
     def is_ascii(s):
         """Check if a given string is ASCII."""
         return s.isascii()
 else:
     def is_ascii(s):
         """Check if a given string is ASCII."""
         # this version is for old Pythons
-        for c in s: 
-            if c > '\x7f': 
-                return False 
-        return True 
+        for c in s:
+            if c > '\x7f':
+                return False
+        return True
 
 def has_foreign_lemma(word):
     """Check if a word (node) has a foreign lemma.
 
     In UniDic, these lemmas don't get their own field, instead the lemma field
     is overloaded. There are also cases where the lemma field is overloaded
     with non-foreign-lemma information.
     """
 
-    if '-' in word.surface: 
+    if '-' in word.surface:
         # TODO check if this is actually possible in vanilla unidic
         return False
 
     if not word.feature.lemma:
         # No lemma means no foreign lemma
         return False
 
@@ -116,16 +116,16 @@
 
         # these are too minor to be worth exposing as arguments
         self.use_tch = (self.system in ('hepburn',))
         self.use_wa  = (self.system in ('hepburn', 'kunrei'))
         self.use_he  = (self.system in ('nihon',))
         self.use_wo  = (self.system in ('hepburn', 'nihon'))
 
-        self.use_foreign_spelling = True
-        self.ensure_ascii = True
+        self.use_foreign_spelling = use_foreign_spelling
+        self.ensure_ascii = ensure_ascii
 
     def add_exception(self, key, val):
         """Add an exception to the internal list.
 
         An exception overrides a whole token, for example to replace "Toukyou"
         with "Tokyo". Note that it must match the tokenizer output and be a
         single token to work. To replace longer phrases, you'll need to use a
@@ -203,15 +203,15 @@
 
             # resolve split verbs / adjectives
             roma = self.romaji_word(word)
             if roma and out and out[-1] == 'っ':
                 out = out[:-1] + roma[0]
             if word.feature.pos2 == '固有名詞':
                 roma = roma.title()
-            if (title and 
+            if (title and
                 word.feature.pos1 not in ('助詞', '助動詞', '接尾辞') and
                 not (pw and pw.feature.pos1 == '接頭辞')):
                 roma = roma.title()
             # handle punctuation with atypical spacing
             if word.surface in '「『':
                 out += ' ' + roma
                 continue
@@ -229,15 +229,15 @@
             # 今日、 -> kyou, ; 図書館 -> toshokan
             if nw and nw.feature.pos1 in ('補助記号', '接尾辞'): continue
             # special case for half-width commas
             if nw and nw.surface == ',': continue
             # 思えば -> omoeba
             if nw and nw.feature.pos2 in ('接続助詞'): continue
             # 333 -> 333 ; this should probably be handled in mecab
-            if (word.surface.isdigit() and 
+            if (word.surface.isdigit() and
                     nw and nw.surface.isdigit()):
                 continue
             # そうでした -> sou deshita
             if (nw and word.feature.pos1 in ('動詞', '助動詞','形容詞')
                    and nw.feature.pos1 == '助動詞'
                    and nw.surface != 'です'):
                 continue
@@ -263,15 +263,15 @@
 
         if is_ascii(word.surface):
             return word.surface
 
         # deal with unks first
         if word.is_unk:
             # at this point is is presumably an unk
-            # Check character type using the values defined in char.def. 
+            # Check character type using the values defined in char.def.
             # This is constant across unidic versions so far but not guaranteed.
             if word.char_type == 6 or word.char_type == 7: # hiragana/katakana
                 kana = jaconv.kata2hira(word.surface)
                 return self.map_kana(kana)
 
             # At this point this is an unknown word and not kana. Could be
             # unknown kanji, could be hangul, cyrillic, something else.
@@ -281,24 +281,24 @@
                 return out
             else:
                 return word.surface
 
         if word.feature.pos1 == '補助記号':
             # If it's punctuation we don't recognize, just discard it
             return self.table.get(word.surface, '')
-        elif (self.use_wa and 
+        elif (self.use_wa and
                 word.feature.pos1 == '助詞' and word.feature.pron == 'ワ'):
             return 'wa'
-        elif (not self.use_he and 
+        elif (not self.use_he and
                 word.feature.pos1 == '助詞' and word.feature.pron == 'エ'):
             return 'e'
-        elif (not self.use_wo and 
+        elif (not self.use_wo and
                 word.feature.pos1 == '助詞' and word.feature.pron == 'オ'):
             return 'o'
-        elif (self.use_foreign_spelling and 
+        elif (self.use_foreign_spelling and
                 has_foreign_lemma(word)):
             # this is a foreign word with known spelling
             return word.feature.lemma.split('-')[-1]
         elif word.feature.kana:
             # for known words
             kana = jaconv.kata2hira(word.feature.kana)
             return self.map_kana(kana)
@@ -320,28 +320,28 @@
         return out
 
     def get_single_mapping(self, pk, kk, nk):
         """Given a single kana and its neighbors, return the mapped romaji."""
         # handle odoriji
         # NOTE: This is very rarely useful at present because odoriji are not
         # left in readings for dictionary words, and we can't follow kana
-        # across word boundaries. 
+        # across word boundaries.
         if kk in ODORI:
             if kk in 'ゝヽ':
                 if pk: return pk
                 else: return '' # invalid but be nice
             if kk in 'ゞヾ': # repeat with voicing
                 if not pk: return ''
                 vv = add_dakuten(pk)
                 if vv: return self.table[vv]
                 else: return ''
             # remaining are 々 for kanji and 〃 for symbols, but we can't
             # infer their span reliably (or handle rendaku)
             return ''
-        
+
 
         # handle digraphs
         if pk and (pk + kk) in self.table:
             return self.table[pk + kk]
         if nk and (kk + nk) in self.table:
             return ''
 
@@ -350,21 +350,21 @@
             return self.table[kk][:-1] + self.table[nk]
         if kk in SUTEGANA:
             return ''
 
         if kk == 'ー': # 長音符
             if pk and pk in self.table: return self.table[pk][-1]
             else: return '-'
-        
+
         if kk == 'っ':
             if nk:
                 if self.use_tch and nk == 'ち': return 't'
                 elif nk in 'あいうえおっ': return '-'
                 else: return self.table[nk][0] # first character
-            else: 
+            else:
                 # seems like it should never happen, but 乗っ|た is two tokens
                 # so leave this as is and pick it up at the word level
                 return 'っ'
 
         if kk == 'ん':
             if nk and nk in 'あいうえおやゆよ': return "n'"
             else: return 'n'
```

### Comparing `cutlet-0.2.0/cutlet/mapping.py` & `cutlet-0.2.1/cutlet/mapping.py`

 * *Files identical despite different names*

### Comparing `cutlet-0.2.0/cutlet/test/blns.json` & `cutlet-0.2.1/cutlet/test/blns.json`

 * *Files identical despite different names*

### Comparing `cutlet-0.2.0/cutlet/test/test_basic.py` & `cutlet-0.2.1/cutlet/test/test_basic.py`

 * *Files identical despite different names*

### Comparing `cutlet-0.2.0/cutlet/test/test_fuzz.py` & `cutlet-0.2.1/cutlet/test/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `cutlet-0.2.0/cutlet.egg-info/PKG-INFO` & `cutlet-0.2.1/cutlet.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cutlet
-Version: 0.2.0
+Version: 0.2.1
 Summary: Romaji converter
 Home-page: https://github.com/polm/cutlet
 Author: Paul O'Leary McCann
 Author-email: polm@dampfkraft.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Japanese
 Requires-Python: >=3.5
@@ -14,15 +14,15 @@
 [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://share.streamlit.io/polm/cutlet-demo/main/demo.py)
 [![Current PyPI packages](https://badge.fury.io/py/cutlet.svg)](https://pypi.org/project/cutlet/)
 
 # cutlet
 
 <img src="https://github.com/polm/cutlet/raw/master/cutlet.png" width=125 height=125 alt="cutlet by Irasutoya" />
 
-Cutlet is a tool to convert Japanese to romaji. Check out the [interactive demo][demo]!
+Cutlet is a tool to convert Japanese to romaji. Check out the [interactive demo][demo]! Also see the [docs](https://polm.github.io/cutlet/cutlet.html) and the [original blog post](https://www.dampfkraft.com/nlp/cutlet-python-romaji-converter.html). 
 
 [demo]: https://share.streamlit.io/polm/cutlet-demo/main/demo.py
 
 **issueを英語で書く必要はありません。**
 
 Features:
```

### Comparing `cutlet-0.2.0/cutlet.egg-info/SOURCES.txt` & `cutlet-0.2.1/cutlet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cutlet-0.2.0/cutlet.png` & `cutlet-0.2.1/cutlet.png`

 * *Files identical despite different names*

### Comparing `cutlet-0.2.0/docs/cutlet.html` & `cutlet-0.2.1/docs/cutlet.html`

 * *Files identical despite different names*

### Comparing `cutlet-0.2.0/docs/search.js` & `cutlet-0.2.1/docs/search.js`

 * *Files identical despite different names*

### Comparing `cutlet-0.2.0/setup.py` & `cutlet-0.2.1/setup.py`

 * *Files identical despite different names*

