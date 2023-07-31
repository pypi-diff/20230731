# Comparing `tmp/sentibank-0.0.1.2.tar.gz` & `tmp/sentibank-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentibank-0.0.1.2.tar", last modified: Mon Jul 31 17:13:43 2023, max compression
+gzip compressed data, was "sentibank-0.0.1.3.tar", last modified: Mon Jul 31 17:34:32 2023, max compression
```

## Comparing `sentibank-0.0.1.2.tar` & `sentibank-0.0.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 17:13:43.006034 sentibank-0.0.1.2/
--rw-rw-rw-   0        0        0     1084 2023-07-31 16:51:12.000000 sentibank-0.0.1.2/LICENSE
--rw-rw-rw-   0        0        0       40 2023-07-31 16:54:25.000000 sentibank-0.0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      416 2023-07-31 17:13:43.006034 sentibank-0.0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       99 2023-07-31 16:51:12.000000 sentibank-0.0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 17:13:42.970034 sentibank-0.0.1.2/sentibank/
--rw-rw-rw-   0        0        0        0 2023-07-31 17:01:20.000000 sentibank-0.0.1.2/sentibank/__init__.py
--rw-rw-rw-   0        0        0     2566 2023-07-31 17:07:44.000000 sentibank-0.0.1.2/sentibank/archive.py
-drwxrwxrwx   0        0        0        0 2023-07-31 17:13:42.985034 sentibank-0.0.1.2/sentibank/dict_arXiv/
-drwxrwxrwx   0        0        0        0 2023-07-31 17:13:42.987033 sentibank-0.0.1.2/sentibank/dict_arXiv/AFINN/
--rw-rw-rw-   0        0        0    42865 2023-07-25 14:30:20.000000 sentibank-0.0.1.2/sentibank/dict_arXiv/AFINN/AFINN_v2015.csv
--rw-rw-rw-   0        0        0    60808 2023-07-16 07:07:32.000000 sentibank-0.0.1.2/sentibank/dict_arXiv/AFINN/AFINN_v2015.pickle
-drwxrwxrwx   0        0        0        0 2023-07-31 17:13:42.989033 sentibank-0.0.1.2/sentibank/dict_arXiv/Aigents/
--rw-rw-rw-   0        0        0   291231 2023-07-25 14:32:19.000000 sentibank-0.0.1.2/sentibank/dict_arXiv/Aigents/Aigents+_v2022.csv
--rw-rw-rw-   0        0        0   218491 2023-07-25 14:28:33.000000 sentibank-0.0.1.2/sentibank/dict_arXiv/Aigents/Aigents+_v2022.pickle
-drwxrwxrwx   0        0        0        0 2023-07-31 17:13:43.002042 sentibank-0.0.1.2/sentibank/dict_arXiv/MASTER/
--rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 sentibank-0.0.1.2/sentibank/dict_arXiv/MASTER/MASTER_v2022.csv
--rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 sentibank-0.0.1.2/sentibank/dict_arXiv/MASTER/MASTER_v2022.pickle
-drwxrwxrwx   0        0        0        0 2023-07-31 17:13:43.004033 sentibank-0.0.1.2/sentibank/dict_arXiv/VADER/
--rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 sentibank-0.0.1.2/sentibank/dict_arXiv/VADER/VADER_v2014.csv
--rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 sentibank-0.0.1.2/sentibank/dict_arXiv/VADER/VADER_v2014_mod.pickle
--rw-rw-rw-   0        0        0     3071 2023-07-25 14:11:12.000000 sentibank-0.0.1.2/sentibank/dict_arXiv/emos.py
--rw-rw-rw-   0        0        0     8743 2023-07-31 17:13:06.000000 sentibank-0.0.1.2/sentibank/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 17:13:42.984034 sentibank-0.0.1.2/sentibank.egg-info/
--rw-rw-rw-   0        0        0      416 2023-07-31 17:13:42.000000 sentibank-0.0.1.2/sentibank.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      677 2023-07-31 17:13:42.000000 sentibank-0.0.1.2/sentibank.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 17:13:42.000000 sentibank-0.0.1.2/sentibank.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-07-31 17:13:42.000000 sentibank-0.0.1.2/sentibank.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-31 17:13:42.000000 sentibank-0.0.1.2/sentibank.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-31 17:13:43.007044 sentibank-0.0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-07-31 17:13:29.000000 sentibank-0.0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 17:34:32.791133 sentibank-0.0.1.3/
+-rw-rw-rw-   0        0        0     1084 2023-07-31 16:51:12.000000 sentibank-0.0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       40 2023-07-31 16:54:25.000000 sentibank-0.0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      416 2023-07-31 17:34:32.791133 sentibank-0.0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       99 2023-07-31 16:51:12.000000 sentibank-0.0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 17:34:32.756132 sentibank-0.0.1.3/sentibank/
+-rw-rw-rw-   0        0        0        0 2023-07-31 17:01:20.000000 sentibank-0.0.1.3/sentibank/__init__.py
+-rw-rw-rw-   0        0        0     2566 2023-07-31 17:07:44.000000 sentibank-0.0.1.3/sentibank/archive.py
+drwxrwxrwx   0        0        0        0 2023-07-31 17:34:32.770131 sentibank-0.0.1.3/sentibank/dict_arXiv/
+drwxrwxrwx   0        0        0        0 2023-07-31 17:34:32.772131 sentibank-0.0.1.3/sentibank/dict_arXiv/AFINN/
+-rw-rw-rw-   0        0        0    42865 2023-07-25 14:30:20.000000 sentibank-0.0.1.3/sentibank/dict_arXiv/AFINN/AFINN_v2015.csv
+-rw-rw-rw-   0        0        0    60808 2023-07-16 07:07:32.000000 sentibank-0.0.1.3/sentibank/dict_arXiv/AFINN/AFINN_v2015.pickle
+drwxrwxrwx   0        0        0        0 2023-07-31 17:34:32.774131 sentibank-0.0.1.3/sentibank/dict_arXiv/Aigents/
+-rw-rw-rw-   0        0        0   291231 2023-07-25 14:32:19.000000 sentibank-0.0.1.3/sentibank/dict_arXiv/Aigents/Aigents+_v2022.csv
+-rw-rw-rw-   0        0        0   218491 2023-07-25 14:28:33.000000 sentibank-0.0.1.3/sentibank/dict_arXiv/Aigents/Aigents+_v2022.pickle
+drwxrwxrwx   0        0        0        0 2023-07-31 17:34:32.787142 sentibank-0.0.1.3/sentibank/dict_arXiv/MASTER/
+-rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 sentibank-0.0.1.3/sentibank/dict_arXiv/MASTER/MASTER_v2022.csv
+-rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 sentibank-0.0.1.3/sentibank/dict_arXiv/MASTER/MASTER_v2022.pickle
+drwxrwxrwx   0        0        0        0 2023-07-31 17:34:32.790143 sentibank-0.0.1.3/sentibank/dict_arXiv/VADER/
+-rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 sentibank-0.0.1.3/sentibank/dict_arXiv/VADER/VADER_v2014.csv
+-rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 sentibank-0.0.1.3/sentibank/dict_arXiv/VADER/VADER_v2014_mod.pickle
+-rw-rw-rw-   0        0        0     3071 2023-07-25 14:11:12.000000 sentibank-0.0.1.3/sentibank/dict_arXiv/emos.py
+-rw-rw-rw-   0        0        0     9291 2023-07-31 17:20:48.000000 sentibank-0.0.1.3/sentibank/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 17:34:32.769132 sentibank-0.0.1.3/sentibank.egg-info/
+-rw-rw-rw-   0        0        0      416 2023-07-31 17:34:32.000000 sentibank-0.0.1.3/sentibank.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      677 2023-07-31 17:34:32.000000 sentibank-0.0.1.3/sentibank.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 17:34:32.000000 sentibank-0.0.1.3/sentibank.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-31 17:34:32.000000 sentibank-0.0.1.3/sentibank.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-31 17:34:32.000000 sentibank-0.0.1.3/sentibank.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-31 17:34:32.792143 sentibank-0.0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-07-31 17:34:20.000000 sentibank-0.0.1.3/setup.py
```

### Comparing `sentibank-0.0.1.2/LICENSE` & `sentibank-0.0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1.2/sentibank/archive.py` & `sentibank-0.0.1.3/sentibank/archive.py`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1.2/sentibank/dict_arXiv/AFINN/AFINN_v2015.csv` & `sentibank-0.0.1.3/sentibank/dict_arXiv/AFINN/AFINN_v2015.csv`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1.2/sentibank/dict_arXiv/AFINN/AFINN_v2015.pickle` & `sentibank-0.0.1.3/sentibank/dict_arXiv/AFINN/AFINN_v2015.pickle`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1.2/sentibank/dict_arXiv/Aigents/Aigents+_v2022.csv` & `sentibank-0.0.1.3/sentibank/dict_arXiv/Aigents/Aigents+_v2022.csv`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1.2/sentibank/dict_arXiv/Aigents/Aigents+_v2022.pickle` & `sentibank-0.0.1.3/sentibank/dict_arXiv/Aigents/Aigents+_v2022.pickle`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1.2/sentibank/dict_arXiv/MASTER/MASTER_v2022.csv` & `sentibank-0.0.1.3/sentibank/dict_arXiv/MASTER/MASTER_v2022.csv`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1.2/sentibank/dict_arXiv/MASTER/MASTER_v2022.pickle` & `sentibank-0.0.1.3/sentibank/dict_arXiv/MASTER/MASTER_v2022.pickle`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1.2/sentibank/dict_arXiv/VADER/VADER_v2014.csv` & `sentibank-0.0.1.3/sentibank/dict_arXiv/VADER/VADER_v2014.csv`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1.2/sentibank/dict_arXiv/VADER/VADER_v2014_mod.pickle` & `sentibank-0.0.1.3/sentibank/dict_arXiv/VADER/VADER_v2014_mod.pickle`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1.2/sentibank/dict_arXiv/emos.py` & `sentibank-0.0.1.3/sentibank/dict_arXiv/emos.py`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1.2/sentibank/utils.py` & `sentibank-0.0.1.3/sentibank/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -217,22 +217,30 @@
                 general_dict["emos"] += value
             elif key == "EMOJI":
                 general_dict["emos"] += value
             else:
                 misc.append(key)
                 general_dict["miscellaneous"] += value
 
-        granular_dict = dict(
-            ("{} ({})".format(key, spacy.explain(key)), value)
-            for (key, value) in granular_dict.items()
-        )
+        granular_dict_adv = {} 
+        
+        if "EMOTICON" or "EMOJI" in granular_dict.keys(): 
+            for key, value in granular_dict.items(): 
+                if key == "EMOTICON": 
+                    granular_dict_adv["EMOTICON (textual representations of emotions)"] = value
+                elif key == "EMOJI": 
+                    granular_dict_adv["EMOJI (pictorial symbols of emotions, objects, or concepts)"] = value 
+                else: 
+                    granular_dict_adv["{} ({})".format(key,spacy.explain(key))] = value
+        else: 
+            granular_dict_adv = dict(("{} ({})".format(key,spacy.explain(key)), value) for (key, value) in granular_dict.items())
 
         part_of_speech = {
             "general": self.sort_dict(general_dict),
-            "granular": self.sort_dict(granular_dict),
+            "granular": self.sort_dict(granular_dict_adv),
             "misc": misc,
         }
 
         summary = {
             "Dictionary Type": lex_dict_type,
             "Sentiment Score": score_summary,
             "Sentiment Lexicon": part_of_speech,
```

### Comparing `sentibank-0.0.1.2/sentibank.egg-info/SOURCES.txt` & `sentibank-0.0.1.3/sentibank.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1.2/setup.py` & `sentibank-0.0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'sentibank', 
   packages = ['sentibank'],   
-  version = '0.0.1.2',      
+  version = '0.0.1.3',      
   license='MIT',        
   description = 'TYPE YOUR DESCRIPTION HERE',   
   author = 'Nick S.H Oh',                   
   author_email = 'nick.sh.oh@socialscience.ai',      
   url = 'https://github.com/socius-org/sentibank',  
-  download_url = 'https://github.com/socius-org/sentibank/archive/refs/tags/0.0.1.2.tar.gz', 
+  download_url = 'https://github.com/socius-org/sentibank/archive/refs/tags/0.0.1.3.tar.gz', 
   keywords = ['AI', 'Social Science', 'Sentiment Analysis'],   # Keywords that define your package best
   install_requires=[
           'spacy',
           'spacymoji',
           'rich'
       ],
   include_package_data=True
```

