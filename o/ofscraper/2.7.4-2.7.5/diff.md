# Comparing `tmp/ofscraper-2.7.4.tar.gz` & `tmp/ofscraper-2.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-2.7.4.tar", max compression
+gzip compressed data, was "ofscraper-2.7.5.tar", max compression
```

## Comparing `ofscraper-2.7.4.tar` & `ofscraper-2.7.5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1067 2023-07-31 00:55:32.542194 ofscraper-2.7.4/LICENSE
--rw-r--r--   0        0        0     2859 2023-07-31 00:55:32.542194 ofscraper-2.7.4/README.md
--rw-r--r--   0        0        0      607 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/__init__.py
--rw-r--r--   0        0        0     1016 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/__version__.py
--rw-r--r--   0        0        0      999 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/__version__.pye
--rw-r--r--   0        0        0        1 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/api/__init__.py
--rw-r--r--   0        0        0     8591 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/api/archive.py
--rw-r--r--   0        0        0     9690 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1060 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/api/init.py
--rw-r--r--   0        0        0     7357 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/api/labels.py
--rw-r--r--   0        0        0     3246 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/api/me.py
--rw-r--r--   0        0        0     9415 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/api/messages.py
--rw-r--r--   0        0        0     9499 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/api/paid.py
--rw-r--r--   0        0        0     5645 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/api/pinned.py
--rw-r--r--   0        0        0     4393 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/api/profile.py
--rw-r--r--   0        0        0     3294 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     9141 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/api/timeline.py
--rw-r--r--   0        0        0        0 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/classes/__init__.py
--rw-r--r--   0        0        0      804 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/classes/labels.py
--rw-r--r--   0        0        0     8491 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/classes/media.py
--rw-r--r--   0        0        0     7278 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/classes/placeholder.py
--rw-r--r--   0        0        0     3737 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/classes/posts.py
--rw-r--r--   0        0        0     4656 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/classes/sessionbuilder.py
--rw-r--r--   0        0        0    29810 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/classes/table.py
--rw-r--r--   0        0        0    14593 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/commands/check.py
--rw-r--r--   0        0        0     5353 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/commands/manual.py
--rwxr-xr-x   0        0        0    14111 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0     6917 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/db/__init__.py
--rw-r--r--   0        0        0    10059 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3576 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-07-31 00:55:32.550193 ofscraper-2.7.4/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     4891 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/interaction/like.py
--rw-r--r--   0        0        0      730 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/prompts/keybindings.py
--rw-r--r--   0        0        0     5794 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/prompts/promptConvert.py
--rw-r--r--   0        0        0     6695 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0     7834 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0    29163 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0     1583 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/start.py
--rw-r--r--   0        0        0        1 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0    12396 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/utils/args.py
--rw-r--r--   0        0        0     9965 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/utils/auth.py
--rw-r--r--   0        0        0     8977 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0    13582 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/utils/config.py
--rw-r--r--   0        0        0      257 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/utils/console.py
--rw-r--r--   0        0        0     1080 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    24662 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     2865 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     5564 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/utils/filters.py
--rw-r--r--   0        0        0     7300 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/utils/logger.py
--rw-r--r--   0        0        0    10686 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/utils/of.py
--rw-r--r--   0        0        0     7013 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     4263 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      399 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/utils/semaphoreDelayed.py
--rw-r--r--   0        0        0     1211 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/utils/separate.py
--rw-r--r--   0        0        0      554 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/utils/stdout.py
--rw-r--r--   0        0        0     5638 2023-07-31 00:55:32.554193 ofscraper-2.7.4/ofscraper/utils/userselector.py
--rw-r--r--   0        0        0     1967 2023-07-31 00:56:12.822452 ofscraper-2.7.4/pyproject.toml
--rw-r--r--   0        0        0     4594 1970-01-01 00:00:00.000000 ofscraper-2.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-31 01:05:30.029800 ofscraper-2.7.5/LICENSE
+-rw-r--r--   0        0        0     2859 2023-07-31 01:05:30.029800 ofscraper-2.7.5/README.md
+-rw-r--r--   0        0        0      607 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/__init__.py
+-rw-r--r--   0        0        0     1016 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/__version__.py
+-rw-r--r--   0        0        0      999 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/__version__.pye
+-rw-r--r--   0        0        0        1 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/__init__.py
+-rw-r--r--   0        0        0     8591 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/archive.py
+-rw-r--r--   0        0        0     9690 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1060 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/init.py
+-rw-r--r--   0        0        0     7357 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/labels.py
+-rw-r--r--   0        0        0     3246 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/me.py
+-rw-r--r--   0        0        0     9415 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/messages.py
+-rw-r--r--   0        0        0     9499 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     5645 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0     4393 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     3294 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     9141 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0        0 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/classes/__init__.py
+-rw-r--r--   0        0        0      804 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/classes/labels.py
+-rw-r--r--   0        0        0     8491 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/classes/media.py
+-rw-r--r--   0        0        0     7278 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/classes/placeholder.py
+-rw-r--r--   0        0        0     3737 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/classes/posts.py
+-rw-r--r--   0        0        0     4656 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/classes/sessionbuilder.py
+-rw-r--r--   0        0        0    29810 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/classes/table.py
+-rw-r--r--   0        0        0    14593 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/commands/check.py
+-rw-r--r--   0        0        0     5353 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/commands/manual.py
+-rwxr-xr-x   0        0        0    14111 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0     6936 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0    10059 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3576 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     4891 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0      730 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/prompts/keybindings.py
+-rw-r--r--   0        0        0     5794 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/prompts/promptConvert.py
+-rw-r--r--   0        0        0     6695 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0     7834 2023-07-31 01:05:30.037800 ofscraper-2.7.5/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0    29433 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0     1583 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/start.py
+-rw-r--r--   0        0        0        1 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0    12404 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/args.py
+-rw-r--r--   0        0        0     9965 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0     8977 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0    13774 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      257 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/console.py
+-rw-r--r--   0        0        0     1080 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    28038 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     2865 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     5564 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0     7300 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0    10686 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/of.py
+-rw-r--r--   0        0        0     7013 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     4263 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      399 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/semaphoreDelayed.py
+-rw-r--r--   0        0        0     1211 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0      554 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/stdout.py
+-rw-r--r--   0        0        0     5638 2023-07-31 01:05:30.041800 ofscraper-2.7.5/ofscraper/utils/userselector.py
+-rw-r--r--   0        0        0     1967 2023-07-31 01:06:03.562448 ofscraper-2.7.5/pyproject.toml
+-rw-r--r--   0        0        0     4594 1970-01-01 00:00:00.000000 ofscraper-2.7.5/PKG-INFO
```

### Comparing `ofscraper-2.7.4/LICENSE` & `ofscraper-2.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/README.md` & `ofscraper-2.7.5/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/__init__.py` & `ofscraper-2.7.5/ofscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/__version__.py` & `ofscraper-2.7.5/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/__version__.pye` & `ofscraper-2.7.5/ofscraper/__version__.pye`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/api/archive.py` & `ofscraper-2.7.5/ofscraper/api/archive.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/api/highlights.py` & `ofscraper-2.7.5/ofscraper/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/api/init.py` & `ofscraper-2.7.5/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/api/labels.py` & `ofscraper-2.7.5/ofscraper/api/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/api/me.py` & `ofscraper-2.7.5/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/api/messages.py` & `ofscraper-2.7.5/ofscraper/api/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/api/paid.py` & `ofscraper-2.7.5/ofscraper/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/api/pinned.py` & `ofscraper-2.7.5/ofscraper/api/pinned.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/api/profile.py` & `ofscraper-2.7.5/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/api/subscriptions.py` & `ofscraper-2.7.5/ofscraper/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/api/timeline.py` & `ofscraper-2.7.5/ofscraper/api/timeline.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/classes/labels.py` & `ofscraper-2.7.5/ofscraper/classes/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/classes/media.py` & `ofscraper-2.7.5/ofscraper/classes/media.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/classes/placeholder.py` & `ofscraper-2.7.5/ofscraper/classes/placeholder.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/classes/posts.py` & `ofscraper-2.7.5/ofscraper/classes/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/classes/sessionbuilder.py` & `ofscraper-2.7.5/ofscraper/classes/sessionbuilder.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/classes/table.py` & `ofscraper-2.7.5/ofscraper/classes/table.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/commands/check.py` & `ofscraper-2.7.5/ofscraper/commands/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/commands/manual.py` & `ofscraper-2.7.5/ofscraper/commands/manual.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/commands/scraper.py` & `ofscraper-2.7.5/ofscraper/commands/scraper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/constants.py` & `ofscraper-2.7.5/ofscraper/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 }
 
 disclaimers = [
 'This tool is not affiliated, associated, or partnered with OnlyFans in any way. We are not authorized, endorsed, or sponsored by OnlyFans. All OnlyFans trademarks remain the property of Fenix International Limited.',
   'This tool is for educational purposes only and is not intended for actual use. Should you choose to actually use it you accept all consequences and agree that you are not using it to redistribute content or  for any other action that will cause loss of revenue to creators or platforms scraped.',
   
 ]
-
+KEY_DEFAULT="keydb"
 DIR_FORMAT_DEFAULT="{model_username}/{responsetype}/{mediatype}/"
 FILE_FORMAT_DEFAULT="{filename}.{ext}"
 METADATA_DEFAULT="{configpath}/{profile}/.data/{model_username}_{model_id}"
 FILE_SIZE_DEFAULT=0
 TEXTLENGTH_DEFAULT=0
 FILTER_DEFAULT=["Images","Audios","Videos"]
 SAVE_PATH_DEFAULT=str(pathlib.Path.home()/'Data/ofscraper')
```

### Comparing `ofscraper-2.7.4/ofscraper/db/operations.py` & `ofscraper-2.7.5/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/db/queries.py` & `ofscraper-2.7.5/ofscraper/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/interaction/like.py` & `ofscraper-2.7.5/ofscraper/interaction/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/prompts/keybindings.py` & `ofscraper-2.7.5/ofscraper/prompts/keybindings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/prompts/promptConvert.py` & `ofscraper-2.7.5/ofscraper/prompts/promptConvert.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/prompts/prompt_strings.py` & `ofscraper-2.7.5/ofscraper/prompts/prompt_strings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/prompts/prompt_validators.py` & `ofscraper-2.7.5/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/prompts/prompts.py` & `ofscraper-2.7.5/ofscraper/prompts/prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,17 +333,24 @@
             'choices':["deviint","digitalcriminals"],
         },
         {
             'type': 'list',
             'name': 'key-mode-default',
             'message': 'Make selection for how to retrive keys',
             'default': config.get_key_mode(config_),
-            'choices':["auto","manual"],
+            'choices':["auto","cdrm","keydb"],
 
         },
+          {
+            'type': 'input',
+            'name': 'keydb_api',
+            'message': 'keydb api key:\n',
+            "long_instruction":"Required if your using keydb for key-mode",
+            'default': config.get_keydb_api(config_) or "",
+        },
 
         {
             'type': 'filepath',
             'name': 'client-id',
             'message': 'Enter path to client id file',
             'default': config.get_client_id(config_) or "",
         },
```

### Comparing `ofscraper-2.7.4/ofscraper/start.py` & `ofscraper-2.7.5/ofscraper/start.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/utils/args.py` & `ofscraper-2.7.5/ofscraper/utils/args.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     advanced.add_argument(
         '-uf', '--users-first', help = 'Scrape all users first rather then one at a time. This only effects downloading posts',default=False,required=False,action="store_true"
     )
     advanced.add_argument(
         '-nc', '--no-cache', help = 'disable cache',default=False,required=False,action="store_true"
     )
     advanced.add_argument(
-        '-k', '--key-mode', help = 'key mode override',default=None,required=False,choices=["auto","manual"],type=str.lower)
+        '-k', '--key-mode', help = 'key mode override',default=None,required=False,choices=["cdrm","manual","keydb"],type=str.lower)
     advanced.add_argument(
         '-dr', '--dynamic-rules', help = 'Dynamic signing',default=None,required=False,choices=["dc","deviint"],type=str.lower)
     advanced.add_argument(
         '-pc', '--part-cleanup', help = 'Cleanup temp .part files\nNote this removes the ability to resume from downloads',default=False,action="store_true")
```

### Comparing `ofscraper-2.7.4/ofscraper/utils/auth.py` & `ofscraper-2.7.5/ofscraper/utils/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/utils/binaries.py` & `ofscraper-2.7.5/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/utils/config.py` & `ofscraper-2.7.5/ofscraper/utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,15 @@
             "custom":get_custom(config),
             "mp4decrypt":get_mp4decrypt(config),
             "ffmpeg":get_ffmpeg(config),
              "discord":get_discord(config),
              "private-key":get_private_key(config),
              "client-id":get_client_id(config),
             "key-mode-default":get_key_mode(config),
+              "keydb_api":get_keydb_api(config),
             "dynamic-mode-default":get_dynamic(config),
             "partfileclean":get_part_file_clean(config),
             "backend":get_backend(config),
 
             "responsetype":{
            "timeline":get_timeline_responsetype(config),
          "message":get_messages_responsetype(config),
@@ -367,18 +368,21 @@
 def get_client_id(config=None):
     if config==None:
         return None 
     return config.get('client-id')
 
 def get_key_mode(config=None):
     if config==None:
-        return "auto" 
+        return constants.KEY_DEFAULT
     value=config.get("key-mode-default")
-    return value.lower() if value and value.lower() in set(["auto","manual"]) else "auto"
-
+    return value.lower() if value and value.lower() in set(["auto","manual"]) else constants.KEY_DEFAULT
+def get_keydb_api(config=None):
+    if config==None:
+        return ""
+    return config.get("keydb_api","") or ""
 def get_dynamic(config=None):
     if config==None:
         return constants.DYNAMIC_DEFAULT
     value=config.get("dynamic-mode-default")
     return value.lower() if value and value.lower() in set(["deviint","dc"]) else "deviint"
 def get_part_file_clean(config=None):
     if config==None:
```

### Comparing `ofscraper-2.7.4/ofscraper/utils/dates.py` & `ofscraper-2.7.5/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/utils/download.py` & `ofscraper-2.7.5/ofscraper/utils/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 from pywidevine.pssh import PSSH
 import arrow
 from bs4 import BeautifulSoup
 try:
     from win32_setctime import setctime  # pylint: disable=import-error
 except ModuleNotFoundError:
     pass
-from tenacity import retry,stop_after_attempt,wait_random
+from tenacity import retry,stop_after_attempt,wait_random,retry_if_not_exception_type
 
 import ofscraper.utils.config as config_
 import ofscraper.utils.separate as seperate
 import ofscraper.db.operations as operations
 import ofscraper.utils.paths as paths
 import ofscraper.utils.auth as auth
 import ofscraper.constants as constants
@@ -263,17 +263,19 @@
                 log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {item['path']} was not created") 
                 return "skipped",1
         elif abs(item["total"]-pathlib.Path(item['path']).absolute().stat().st_size)>500:
             log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] {item['name']} size mixmatch target: {item['total']} vs actual: {pathlib.Path(item['path']).absolute().stat().st_size}")   
             return "skipped",1 
                 
     for item in [audio,video]:
-
-        key=await key_helper_manual(c,item["pssh"],ele.license,ele.id)  if (args_.getargs().key_mode or config_.get_key_mode(config_.read_config()) or "auto") == "manual" \
-        else await key_helper(c,item["pssh"],ele.license,ele.id)
+        key=None
+        keymode=(args_.getargs().key_mode or config_.get_key_mode(config_.read_config()) or "auto")
+        if  keymode== "manual": key=await key_helper_manual(c,item["pssh"],ele.license,ele.id)  
+        elif keymode=="keydb":key=await key_helper_keydb(c,item["pssh"],ele.license,ele.id)  
+        else: key=key_helper_cdrm(c,item["pssh"],ele.license,ele.id)  
         if key==None:
             log.debug(f"Media:{ele.id} Post:{ele.postid} Could not get key")
             return "skipped",1 
         log.debug(f"Media:{ele.id} Post:{ele.postid} got key")
         newpath=pathlib.Path(re.sub("\.part$","",str(item["path"]),re.IGNORECASE))
         log.debug(f"Media:{ele.id} Post:{ele.postid} [attempt {attempt.get()}/{constants.NUM_TRIES}] renaming {pathlib.Path(item['path']).absolute()} -> {newpath}")   
         r=subprocess.run([config_.get_mp4decrypt(config_.read_config()),"--key",key,str(item["path"]),str(newpath)],stdout=subprocess.PIPE,stderr=subprocess.PIPE)
@@ -415,15 +417,93 @@
             cache.set(licence_url,out, expire=constants.KEY_EXPIRY)
             cache.close()
         return out
     except Exception as E:
         log.traceback(E)
         log.traceback(traceback.format_exc())
         raise E
-        
+
+@retry(retry=retry_if_not_exception_type(KeyboardInterrupt),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True) 
+async def key_helper_cdrm(c,pssh,licence_url,id):
+    log.debug(f"ID:{id} using cdrm auto key helper")
+    try:
+        out=cache.get(licence_url)
+        log.debug(f"ID:{id} pssh: {pssh!=None}")
+        log.debug(f"ID:{id} licence: {licence_url}")
+        if out!=None:
+            log.debug(f"ID:{id} cdrm auto key helper got key from cache")
+            return out
+        headers=auth.make_headers(auth.read_auth())
+        headers["cookie"]=auth.get_cookies()
+        auth.create_sign(licence_url,headers)
+        json_data = {
+            'license': licence_url,
+            'headers': json.dumps(headers),
+            'pssh': pssh,
+            'buildInfo': '',
+            'proxy': '',
+            'cache': True,
+        }
+        async with c.requests(url='https://cdrm-project.com/wv',method="post",json=json_data)() as r:
+            httpcontent=await r.text_()
+            log.debug(f"ID:{id} key_response: {httpcontent}")
+            soup = BeautifulSoup(httpcontent, 'html.parser')
+            out=soup.find("li").contents[0]
+            cache.set(licence_url,out, expire=constants.KEY_EXPIRY)
+            cache.close()
+        return out
+    except Exception as E:
+        log.traceback(E)
+        log.traceback(traceback.format_exc())
+        raise E       
+
+@retry(retry=retry_if_not_exception_type(KeyboardInterrupt),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True) 
+async def key_helper_keydb(c,pssh,licence_url,id):
+    log.debug(f"ID:{id} using keydb auto key helper")
+    try:
+        out=cache.get(licence_url)
+        log.debug(f"ID:{id} pssh: {pssh!=None}")
+        log.debug(f"ID:{id} licence: {licence_url}")
+        if out!=None:
+            log.debug(f"ID:{id} keydb auto key helper got key from cache")
+            return out
+        headers=auth.make_headers(auth.read_auth())
+        headers["cookie"]=auth.get_cookies()
+        auth.create_sign(licence_url,headers)
+        json_data = {
+            'license_url': licence_url,
+            'headers': json.dumps(headers),
+            'pssh': pssh,
+            'buildInfo': '',
+            'proxy': '',
+            'cache': True,
+        }
+  
+        headers = {
+            "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (Ktesttemp, like Gecko) Chrome/90.0.4430.85 Safari/537.36",
+            "Content-Type": "application/json",
+            "X-API-Key": config_.get_keydb_api(config_.read_config()),
+        }
+   
+
+
+
+
+        async with c.requests(url='https://keysdb.net/api',method="post",json=json_data,headers=headers)() as r:
+            data=await r.json()
+            log.debug(f"keydb json {data}")
+            if  isinstance(data,str): out=data
+            elif  isinstance(data,object): out=data["keys"][0]["key"]
+            cache.set(licence_url,out, expire=constants.KEY_EXPIRY)
+            cache.close()
+        return out
+    except Exception as E:
+        log.traceback(E)
+        log.traceback(traceback.format_exc())
+        raise E  
 
 async def key_helper_manual(c,pssh,licence_url,id):
     log.debug(f"ID:{id} using manual key helper")
     out=cache.get(licence_url)
     if out!=None:
         log.debug(f"ID:{id} manual key helper got key from cache")
         return out
```

### Comparing `ofscraper-2.7.4/ofscraper/utils/encoding.py` & `ofscraper-2.7.5/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/utils/exit.py` & `ofscraper-2.7.5/ofscraper/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/utils/filters.py` & `ofscraper-2.7.5/ofscraper/utils/filters.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/utils/logger.py` & `ofscraper-2.7.5/ofscraper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/utils/of.py` & `ofscraper-2.7.5/ofscraper/utils/of.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/utils/paths.py` & `ofscraper-2.7.5/ofscraper/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/utils/profiles.py` & `ofscraper-2.7.5/ofscraper/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/utils/separate.py` & `ofscraper-2.7.5/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/utils/stdout.py` & `ofscraper-2.7.5/ofscraper/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/ofscraper/utils/userselector.py` & `ofscraper-2.7.5/ofscraper/utils/userselector.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.7.4/pyproject.toml` & `ofscraper-2.7.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "2.7.4"
+version = "2.7.5"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<3.12"
 httpx = {extras = ["http2"], version = "^0.23.3"}
```

### Comparing `ofscraper-2.7.4/PKG-INFO` & `ofscraper-2.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 2.7.4
+Version: 2.7.5
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

