# Comparing `tmp/ofscraper-2.7.5.tar.gz` & `tmp/ofscraper-2.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-2.7.5.tar", max compression
+gzip compressed data, was "ofscraper-2.7.6.tar", max compression
```

## Comparing `ofscraper-2.7.5.tar` & `ofscraper-2.7.6.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1067 2023-07-31 01:05:30.029800 ofscraper-2.7.5/LICENSE
--rw-r--r--   0        0        0     2859 2023-07-31 01:05:30.029800 ofscraper-2.7.5/README.md
--rw-r--r--   0        0        0      607 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/__init__.py
--rw-r--r--   0        0        0     1016 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/__version__.py
--rw-r--r--   0        0        0      999 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/__version__.pye
--rw-r--r--   0        0        0        1 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/__init__.py
--rw-r--r--   0        0        0     8591 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/archive.py
--rw-r--r--   0        0        0     9690 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1060 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/init.py
--rw-r--r--   0        0        0     7357 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/labels.py
--rw-r--r--   0        0        0     3246 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/me.py
--rw-r--r--   0        0        0     9415 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/messages.py
--rw-r--r--   0        0        0     9499 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/paid.py
--rw-r--r--   0        0        0     5645 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/pinned.py
--rw-r--r--   0        0        0     4393 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/profile.py
--rw-r--r--   0        0        0     3294 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     9141 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/timeline.py
--rw-r--r--   0        0        0        0 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/classes/__init__.py
--rw-r--r--   0        0        0      804 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/classes/labels.py
--rw-r--r--   0        0        0     8491 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/classes/media.py
--rw-r--r--   0        0        0     7278 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/classes/placeholder.py
--rw-r--r--   0        0        0     3737 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/classes/posts.py
--rw-r--r--   0        0        0     4656 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/classes/sessionbuilder.py
--rw-r--r--   0        0        0    29810 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/classes/table.py
--rw-r--r--   0        0        0    14593 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/commands/check.py
--rw-r--r--   0        0        0     5353 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/commands/manual.py
--rwxr-xr-x   0        0        0    14111 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0     6936 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/db/__init__.py
--rw-r--r--   0        0        0    10059 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3576 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     4891 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/interaction/like.py
--rw-r--r--   0        0        0      730 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/prompts/keybindings.py
--rw-r--r--   0        0        0     5794 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/prompts/promptConvert.py
--rw-r--r--   0        0        0     6695 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0     7834 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0    29433 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0     1583 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/start.py
--rw-r--r--   0        0        0        1 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0    12404 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/args.py
--rw-r--r--   0        0        0     9965 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/auth.py
--rw-r--r--   0        0        0     8977 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0    13774 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/config.py
--rw-r--r--   0        0        0      257 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/console.py
--rw-r--r--   0        0        0     1080 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    28038 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     2865 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     5564 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/filters.py
--rw-r--r--   0        0        0     7300 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/logger.py
--rw-r--r--   0        0        0    10686 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/of.py
--rw-r--r--   0        0        0     7013 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     4263 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      399 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/semaphoreDelayed.py
--rw-r--r--   0        0        0     1211 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/separate.py
--rw-r--r--   0        0        0      554 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/stdout.py
--rw-r--r--   0        0        0     5638 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/userselector.py
--rw-r--r--   0        0        0     1967 2023-07-31 01:06:03.562448 ofscraper-2.7.5/pyproject.toml
--rw-r--r--   0        0        0     4594 1970-01-01 00:00:00.000000 ofscraper-2.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-31 14:43:25.683700 ofscraper-2.7.6/LICENSE
+-rw-r--r--   0        0        0     2859 2023-07-31 14:43:25.683700 ofscraper-2.7.6/README.md
+-rw-r--r--   0        0        0      607 2023-07-31 14:43:25.687700 ofscraper-2.7.6/ofscraper/__init__.py
+-rw-r--r--   0        0        0     1016 2023-07-31 14:43:25.687700 ofscraper-2.7.6/ofscraper/__version__.py
+-rw-r--r--   0        0        0      999 2023-07-31 14:43:25.687700 ofscraper-2.7.6/ofscraper/__version__.pye
+-rw-r--r--   0        0        0        1 2023-07-31 14:43:25.687700 ofscraper-2.7.6/ofscraper/api/__init__.py
+-rw-r--r--   0        0        0     8591 2023-07-31 14:43:25.687700 ofscraper-2.7.6/ofscraper/api/archive.py
+-rw-r--r--   0        0        0     9690 2023-07-31 14:43:25.687700 ofscraper-2.7.6/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1060 2023-07-31 14:43:25.687700 ofscraper-2.7.6/ofscraper/api/init.py
+-rw-r--r--   0        0        0     7357 2023-07-31 14:43:25.687700 ofscraper-2.7.6/ofscraper/api/labels.py
+-rw-r--r--   0        0        0     3246 2023-07-31 14:43:25.687700 ofscraper-2.7.6/ofscraper/api/me.py
+-rw-r--r--   0        0        0     9415 2023-07-31 14:43:25.687700 ofscraper-2.7.6/ofscraper/api/messages.py
+-rw-r--r--   0        0        0     9499 2023-07-31 14:43:25.687700 ofscraper-2.7.6/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     5645 2023-07-31 14:43:25.687700 ofscraper-2.7.6/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0     4393 2023-07-31 14:43:25.687700 ofscraper-2.7.6/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     3294 2023-07-31 14:43:25.687700 ofscraper-2.7.6/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     9141 2023-07-31 14:43:25.687700 ofscraper-2.7.6/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0        0 2023-07-31 14:43:25.687700 ofscraper-2.7.6/ofscraper/classes/__init__.py
+-rw-r--r--   0        0        0      804 2023-07-31 14:43:25.687700 ofscraper-2.7.6/ofscraper/classes/labels.py
+-rw-r--r--   0        0        0     8491 2023-07-31 14:43:25.687700 ofscraper-2.7.6/ofscraper/classes/media.py
+-rw-r--r--   0        0        0     7278 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/classes/placeholder.py
+-rw-r--r--   0        0        0     3737 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/classes/posts.py
+-rw-r--r--   0        0        0     4656 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/classes/sessionbuilder.py
+-rw-r--r--   0        0        0    29810 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/classes/table.py
+-rw-r--r--   0        0        0    14593 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/commands/check.py
+-rw-r--r--   0        0        0     5353 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/commands/manual.py
+-rwxr-xr-x   0        0        0    14111 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0     6936 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0    10059 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3576 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     4891 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0      730 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/prompts/keybindings.py
+-rw-r--r--   0        0        0     5794 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/prompts/promptConvert.py
+-rw-r--r--   0        0        0     6695 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0     7834 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0    29433 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0     1583 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/start.py
+-rw-r--r--   0        0        0        1 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0    12404 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/utils/args.py
+-rw-r--r--   0        0        0    10197 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0     8977 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0    13774 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      257 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/utils/console.py
+-rw-r--r--   0        0        0     1080 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    28038 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     2865 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     5564 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0     7300 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0    10686 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/utils/of.py
+-rw-r--r--   0        0        0     7013 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     4263 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      399 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/utils/semaphoreDelayed.py
+-rw-r--r--   0        0        0     1211 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0      554 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/utils/stdout.py
+-rw-r--r--   0        0        0     5638 2023-07-31 14:43:25.691700 ofscraper-2.7.6/ofscraper/utils/userselector.py
+-rw-r--r--   0        0        0     1967 2023-07-31 14:44:01.375984 ofscraper-2.7.6/pyproject.toml
+-rw-r--r--   0        0        0     4594 1970-01-01 00:00:00.000000 ofscraper-2.7.6/PKG-INFO
```

### Comparing `ofscraper-2.7.5/LICENSE` & `ofscraper-2.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/README.md` & `ofscraper-2.7.6/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/__init__.py` & `ofscraper-2.7.6/ofscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/__version__.py` & `ofscraper-2.7.6/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/__version__.pye` & `ofscraper-2.7.6/ofscraper/__version__.pye`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/api/archive.py` & `ofscraper-2.7.6/ofscraper/api/archive.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/api/highlights.py` & `ofscraper-2.7.6/ofscraper/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/api/init.py` & `ofscraper-2.7.6/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/api/labels.py` & `ofscraper-2.7.6/ofscraper/api/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/api/me.py` & `ofscraper-2.7.6/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/api/messages.py` & `ofscraper-2.7.6/ofscraper/api/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/api/paid.py` & `ofscraper-2.7.6/ofscraper/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/api/pinned.py` & `ofscraper-2.7.6/ofscraper/api/pinned.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/api/profile.py` & `ofscraper-2.7.6/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/api/subscriptions.py` & `ofscraper-2.7.6/ofscraper/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/api/timeline.py` & `ofscraper-2.7.6/ofscraper/api/timeline.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/classes/labels.py` & `ofscraper-2.7.6/ofscraper/classes/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/classes/media.py` & `ofscraper-2.7.6/ofscraper/classes/media.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/classes/placeholder.py` & `ofscraper-2.7.6/ofscraper/classes/placeholder.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/classes/posts.py` & `ofscraper-2.7.6/ofscraper/classes/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/classes/sessionbuilder.py` & `ofscraper-2.7.6/ofscraper/classes/sessionbuilder.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/classes/table.py` & `ofscraper-2.7.6/ofscraper/classes/table.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/commands/check.py` & `ofscraper-2.7.6/ofscraper/commands/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/commands/manual.py` & `ofscraper-2.7.6/ofscraper/commands/manual.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/commands/scraper.py` & `ofscraper-2.7.6/ofscraper/commands/scraper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/constants.py` & `ofscraper-2.7.6/ofscraper/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/db/operations.py` & `ofscraper-2.7.6/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/db/queries.py` & `ofscraper-2.7.6/ofscraper/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/interaction/like.py` & `ofscraper-2.7.6/ofscraper/interaction/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/prompts/keybindings.py` & `ofscraper-2.7.6/ofscraper/prompts/keybindings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/prompts/promptConvert.py` & `ofscraper-2.7.6/ofscraper/prompts/promptConvert.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/prompts/prompt_strings.py` & `ofscraper-2.7.6/ofscraper/prompts/prompt_strings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/prompts/prompt_validators.py` & `ofscraper-2.7.6/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/prompts/prompts.py` & `ofscraper-2.7.6/ofscraper/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/start.py` & `ofscraper-2.7.6/ofscraper/start.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/utils/args.py` & `ofscraper-2.7.6/ofscraper/utils/args.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/utils/auth.py` & `ofscraper-2.7.6/ofscraper/utils/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,27 +13,30 @@
 import time
 import logging
 from urllib.parse import urlparse
 import requests
 from rich.console import Console
 
 import browser_cookie3
-from .profiles import get_active_profile
-from ..prompts.prompts import *
+
+import ofscraper.prompts.prompts as prompts
 from ..constants import configPath, DIGITALCRIMINALS, requestAuth,DEVIINT
 import ofscraper.utils.paths as paths
 import ofscraper.classes.sessionbuilder as sessionbuilder
+import ofscraper.utils.profiles as profiles
+import ofscraper.utils.args as args_
+import ofscraper.utils.config as config
 
 
 console=Console()
-log=logging.getLogger(__package__)
+log=logging.getLogger("shared")
 
 def read_auth():
     authFile=paths.get_auth_file()
-   
+
     while True:
         try:
             with open(authFile, 'r') as f:
                 authText=f.read()
                 auth = json.loads(authText)
                 for key in list(filter(lambda x:x!="auth_uid_",auth.keys())):
                     if auth[key]==None or  auth[key]=="":
@@ -44,23 +47,23 @@
         except FileNotFoundError:
             console.print(
                 "You don't seem to have an `auth.json` file")
             make_auth()
         except json.JSONDecodeError as e:
             print("You auth.json has a syntax error")
             print(f"{e}\n\n")
-            if reset_auth_prompt():
+            if prompts.reset_auth_prompt():
                 with open( authFile, 'w') as f:
-                    f.write(manual_auth_prompt(authText))
+                    f.write(prompts.manual_auth_prompt(authText))
             else:
                 with open(authFile,"w") as f: 
                     f.write(json.dumps(get_empty()))
 
 
-                
+    make_request_auth()       
     return auth
 
 def get_empty():
     return{
             'auth': {
                 'app-token': '33d57ade8c02dbc5a333db99ff9ae26a',
                 'sess': '',
@@ -81,55 +84,56 @@
             auth = json.loads(authText)
         print("Hint: Select 'Enter Each Field Manually' to edit your current config\n")
         make_auth(auth)
 
         console.print('Your `auth.json` file has been edited.')
     except FileNotFoundError:
         
-        if ask_make_auth_prompt():
+        if prompts.ask_make_auth_prompt():
             make_auth()
     except json.JSONDecodeError as e:
             while True:
                 try:
                     print("You auth.json has a syntax error")
                     print(f"{e}\n\n")
-                    if reset_auth_prompt():
+                    if prompts.reset_auth_prompt():
                         with open( authFile, 'w') as f:
-                            f.write(manual_auth_prompt(authText))
+                            f.write(prompts.manual_auth_prompt(authText))
                     else:
                          with open(authFile,"w"): 
-                            f.write(auth_prompt(get_empty()))
+                            f.write(prompts.auth_prompt(get_empty()))
                     with open(authFile, 'r') as f:
                         authText=f.read()
                         auth = json.loads(authText)
                     break
                 except:
                     continue
+    make_request_auth() 
 
 def make_auth( auth=None):
     authFile=paths.get_auth_file()
     defaultAuth=  get_empty()
 
-    browserSelect=browser_prompt()
+    browserSelect=prompts.browser_prompt()
 
     auth= auth or defaultAuth
     if  browserSelect!="Enter Each Field Manually" and browserSelect!="Paste From M-rcus\' OnlyFans-Cookie-Helper":
         temp=requests.utils.dict_from_cookiejar(getattr(browser_cookie3, browserSelect.lower())(domain_name="onlyfans"))
         auth=auth or  defaultAuth
         for key in ["sess","auth_id","auth_uid_"]:
             auth["auth"][key]=temp.get(key,"")
         console.print("You'll need to go to onlyfans.com and retrive header information\nGo to https://github.com/datawhores/OF-Scraper and find the section named 'Getting Your Auth Info'\nCookie information has been retived automatically\nSo You only need to retrive the x-bc header and the user-agent",style="yellow")
         if not auth["auth"].get("x-bc"):
-            auth["auth"]["x-bc"]=xbc_prompt()
-        auth["auth"]["user_agent"]= user_agent_prompt(auth["auth"].get("user_agent") or "")
+            auth["auth"]["x-bc"]=prompts.xbc_prompt()
+        auth["auth"]["user_agent"]= prompts.user_agent_prompt(auth["auth"].get("user_agent") or "")
 
 
  
     elif browserSelect=="Paste From M-rcus\' OnlyFans-Cookie-Helper":
-        auth=auth_full_paste()
+        auth=prompts.auth_full_paste()
         auth["auth"]["app-token"]="33d57ade8c02dbc5a333db99ff9ae26a"
         for key in ["username","support_2fa","active","email","password","hashed"]:
             auth["auth"].pop(key)
         auth["auth"]["x-bc"]=auth["auth"].pop("x_bc")
         tempCookie=auth["auth"].pop("cookie")
         for ele in tempCookie.split(";"):
             ele=ele.strip(
@@ -142,15 +146,15 @@
             elif ele.find("auth_uid")!=-1:
                 auth["auth"]["auth_uid_"]=ele.replace("auth_uid_","").replace("=","")
            
 
 
     else:
         console.print("You'll need to go to onlyfans.com and retrive header information\nGo to https://github.com/datawhores/OF-Scraper and find the section named 'Getting Your Auth Info'\nYou only need to retrive the x-bc header,the user-agent, and cookie information",style="yellow")
-        auth['auth'].update(auth_prompt(auth['auth']))
+        auth['auth'].update(prompts.auth_prompt(auth['auth']))
     
     console.print(f"{auth}\nWriting to {authFile}",style="yellow")
     with open(authFile, 'w') as f:
         f.write(json.dumps(auth, indent=4))
 
 
 
@@ -225,15 +229,15 @@
             'time': time2
         }
     )
     return headers
 
 
 def read_request_auth() -> dict:
-    profile = get_active_profile()
+    profile = profiles.get_active_profile()
     
 
     p = paths.get_config_home()/profile/ requestAuth
     with open(p, 'r') as f:
         content = json.load(f)
     return content
 
@@ -249,15 +253,15 @@
     # *values, = get_request_auth()
     result = get_request_auth()
     if result:
         *values, = result
 
         request_auth.update(zip(request_auth.keys(), values))
 
-        profile = get_active_profile()
+        profile = profiles.get_active_profile()
 
         p = paths.get_config_home()/profile
         if not p.is_dir():
             p.mkdir(parents=True, exist_ok=True)
 
         with open(p / requestAuth, 'w') as f:
             f.write(json.dumps(request_auth, indent=4))
```

### Comparing `ofscraper-2.7.5/ofscraper/utils/binaries.py` & `ofscraper-2.7.6/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/utils/config.py` & `ofscraper-2.7.6/ofscraper/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/utils/dates.py` & `ofscraper-2.7.6/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/utils/download.py` & `ofscraper-2.7.6/ofscraper/utils/download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/utils/encoding.py` & `ofscraper-2.7.6/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/utils/exit.py` & `ofscraper-2.7.6/ofscraper/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/utils/filters.py` & `ofscraper-2.7.6/ofscraper/utils/filters.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/utils/logger.py` & `ofscraper-2.7.6/ofscraper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/utils/of.py` & `ofscraper-2.7.6/ofscraper/utils/of.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/utils/paths.py` & `ofscraper-2.7.6/ofscraper/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/utils/profiles.py` & `ofscraper-2.7.6/ofscraper/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/utils/separate.py` & `ofscraper-2.7.6/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/utils/stdout.py` & `ofscraper-2.7.6/ofscraper/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/ofscraper/utils/userselector.py` & `ofscraper-2.7.6/ofscraper/utils/userselector.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.5/pyproject.toml` & `ofscraper-2.7.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "2.7.5"
+version = "2.7.6"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<3.12"
 httpx = {extras = ["http2"], version = "^0.23.3"}
```

### Comparing `ofscraper-2.7.5/PKG-INFO` & `ofscraper-2.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 2.7.5
+Version: 2.7.6
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

