# Comparing `tmp/wi1-bot-1.3.5.tar.gz` & `tmp/wi1-bot-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wi1-bot-1.3.5.tar", last modified: Thu Jul 13 05:32:41 2023, max compression
+gzip compressed data, was "wi1-bot-1.3.6.tar", last modified: Mon Jul 31 05:14:41 2023, max compression
```

## Comparing `wi1-bot-1.3.5.tar` & `wi1-bot-1.3.6.tar`

### file list

```diff
@@ -1,52 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:41.497362 wi1-bot-1.3.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/config.yaml.template
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/tests/movie_downloaded.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/wi1_bot/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 05:32:40.000000 wi1-bot-1.3.5/wi1_bot/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/wi1_bot/arr/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/arr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/arr/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/arr/episode.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/arr/movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/arr/radarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/arr/sonarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/wi1_bot/discord/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/discord/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/wi1_bot/discord/cogs/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/discord/cogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/discord/cogs/movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/discord/cogs/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/discord/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/push.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/wi1_bot/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/scripts/add_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/scripts/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/scripts/transcode_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/wi1_bot/transcoder/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/transcoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/transcoder/transcode_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/transcoder/transcoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-13 05:32:26.000000 wi1-bot-1.3.5/wi1_bot/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 05:32:41.501362 wi1-bot-1.3.5/wi1_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-13 05:32:40.000000 wi1-bot-1.3.5/wi1_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-13 05:32:41.000000 wi1-bot-1.3.5/wi1_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 05:32:41.000000 wi1-bot-1.3.5/wi1_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-13 05:32:41.000000 wi1-bot-1.3.5/wi1_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-13 05:32:41.000000 wi1-bot-1.3.5/wi1_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-13 05:32:41.000000 wi1-bot-1.3.5/wi1_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:14:41.895664 wi1-bot-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:14:41.891664 wi1-bot-1.3.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:14:41.891664 wi1-bot-1.3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:14:41.891664 wi1-bot-1.3.6/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-31 05:14:41.895664 wi1-bot-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/config.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 05:14:41.895664 wi1-bot-1.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:14:41.891664 wi1-bot-1.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/tests/movie_downloaded.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:14:41.895664 wi1-bot-1.3.6/wi1_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/wi1_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-31 05:14:41.000000 wi1-bot-1.3.6/wi1_bot/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:14:41.895664 wi1-bot-1.3.6/wi1_bot/arr/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/wi1_bot/arr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/wi1_bot/arr/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/wi1_bot/arr/episode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/wi1_bot/arr/movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/wi1_bot/arr/radarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/wi1_bot/arr/sonarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/wi1_bot/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:14:41.895664 wi1-bot-1.3.6/wi1_bot/discord/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/wi1_bot/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/wi1_bot/discord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:14:41.895664 wi1-bot-1.3.6/wi1_bot/discord/cogs/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/wi1_bot/discord/cogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/wi1_bot/discord/cogs/movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/wi1_bot/discord/cogs/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/wi1_bot/discord/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/wi1_bot/push.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:14:41.895664 wi1-bot-1.3.6/wi1_bot/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/wi1_bot/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/wi1_bot/scripts/add_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/wi1_bot/scripts/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/wi1_bot/scripts/transcode_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:14:41.895664 wi1-bot-1.3.6/wi1_bot/transcoder/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/wi1_bot/transcoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/wi1_bot/transcoder/transcode_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/wi1_bot/transcoder/transcoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-31 05:14:26.000000 wi1-bot-1.3.6/wi1_bot/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:14:41.895664 wi1-bot-1.3.6/wi1_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-31 05:14:41.000000 wi1-bot-1.3.6/wi1_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-31 05:14:41.000000 wi1-bot-1.3.6/wi1_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 05:14:41.000000 wi1-bot-1.3.6/wi1_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-31 05:14:41.000000 wi1-bot-1.3.6/wi1_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-31 05:14:41.000000 wi1-bot-1.3.6/wi1_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 05:14:41.000000 wi1-bot-1.3.6/wi1_bot.egg-info/top_level.txt
```

### Comparing `wi1-bot-1.3.5/.github/workflows/pypi-publish.yml` & `wi1-bot-1.3.6/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.5/.pre-commit-config.yaml` & `wi1-bot-1.3.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.5/LICENSE` & `wi1-bot-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.5/PKG-INFO` & `wi1-bot-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wi1-bot
-Version: 1.3.5
+Version: 1.3.6
 Summary: Discord bot for Radarr/Sonarr integration
 Home-page: https://github.com/wthueb/wi1-bot
 Author-email: William Huebner <wilhueb@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 William Huebner
```

### Comparing `wi1-bot-1.3.5/README.md` & `wi1-bot-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.5/config.yaml.template` & `wi1-bot-1.3.6/config.yaml.template`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.5/pyproject.toml` & `wi1-bot-1.3.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -12,20 +12,20 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10"
 ]
 dynamic = ["version"]
 requires-python = ">=3.10"
 dependencies = [
-    "discord.py==2.2.2",
-    "Flask==2.2.5",
+    "discord.py==2.3.1",
+    "Flask==2.3.2",
     "mongoengine==0.27.0",
-    "pyarr==3.1.3",
-    "PyYAML==6.0",
-    "requests==2.28.2"
+    "pyarr==5.2.0",
+    "PyYAML==6.0.1",
+    "requests==2.31.0"
 ]
 
 [project.optional-dependencies]
 dev = [
     "black==23.3.0",
     "flake8==6.0.0",
     "isort==5.12.0",
```

### Comparing `wi1-bot-1.3.5/wi1_bot/arr/download.py` & `wi1-bot-1.3.6/wi1_bot/arr/download.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.5/wi1_bot/arr/episode.py` & `wi1-bot-1.3.6/wi1_bot/arr/episode.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.5/wi1_bot/arr/movie.py` & `wi1-bot-1.3.6/wi1_bot/arr/movie.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.5/wi1_bot/arr/radarr.py` & `wi1-bot-1.3.6/wi1_bot/arr/sonarr.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,179 +1,197 @@
 from shutil import rmtree
-from typing import Any, cast
+from typing import Any
 
-from pyarr import RadarrAPI
+from pyarr import SonarrAPI
 
 from .download import Download
-from .movie import Movie
 
-json = dict[str, Any]
 
+class Series:
+    def __init__(self, series_json: dict[str, Any]) -> None:
+        self._json = series_json
 
-class Radarr:
+        self.title: str = series_json["title"]
+        self.year: int = series_json["year"]
+        self.tvdb_id: int = series_json["tvdbId"]
+
+        self.db_id: int | None = series_json["id"] if "id" in series_json else None
+
+        self.full_title = f"{self.title} ({self.year})"
+
+        self.url = f"https://thetvdb.com/dereferrer/series/{self.tvdb_id}"
+
+        self.imdb_id = ""
+
+        try:
+            self.imdb_id = series_json["imdbId"]
+            self.url = f"https://imdb.com/title/{self.imdb_id}"
+        except KeyError:
+            pass
+
+    def __str__(self) -> str:
+        return f"[{self.full_title}]({self.url})"
+
+    def __repr__(self) -> str:
+        return str(self.__dict__)
+
+
+class SonarrError(Exception):
+    pass
+
+
+class Sonarr:
     def __init__(self, url: str, api_key: str) -> None:
-        self._radarr = RadarrAPI(url, api_key)
+        self._sonarr = SonarrAPI(url, api_key)
+
+    def lookup_series(self, query: str) -> list[Series]:
+        possible_series = self._sonarr.lookup_series(query)
 
-    def lookup_movie(self, query: str) -> list[Movie]:
-        possible_movies = cast(list[json], self._radarr.lookup_movie(query))
+        if isinstance(possible_series, dict):
+            raise SonarrError(possible_series["message"])
 
-        return [Movie(m) for m in possible_movies]
+        return [Series(s) for s in possible_series]
 
-    def lookup_library(self, query: str) -> list[Movie]:
-        possible_movies = cast(list[json], self._radarr.lookup_movie(query))
+    def lookup_library(self, query: str) -> list[Series]:
+        possible_series = self._sonarr.lookup_series(query)
 
-        return [Movie(m) for m in possible_movies if "id" in m]
+        return [Series(s) for s in possible_series if "id" in s]
 
-    def lookup_user_library(self, query: str, user_id: int) -> list[Movie]:
+    def lookup_user_library(self, query: str, user_id: int) -> list[Series]:
         try:
             tag_id = self._get_tag_for_user_id(user_id)
         except ValueError:
             return []
 
-        tag_detail = cast(dict[str, Any], self._radarr.get_tag_detail(tag_id))
-
-        possible_movies = cast(list[json], self._radarr.lookup_movie(query))
+        possible_series = self._sonarr.lookup_series(query)
 
-        user_movie_ids = tag_detail["movieIds"]
+        # self._sonarr.get_tag_detail is broken/not supported in v1 sonarr API so have
+        # to filter the tmdb lookup (probably slower but saves an API call)
+        user_series = [s for s in possible_series if tag_id in s["tags"]]
 
-        return [
-            Movie(m) for m in possible_movies if "id" in m and m["id"] in user_movie_ids
-        ]
+        return [Series(s) for s in user_series]
 
-    def add_movie(self, movie: Movie, profile: str = "good") -> bool:
-        if self._radarr.get_movie(movie.tmdb_id):
+    def add_series(self, series: Series, profile: str = "good") -> bool:
+        if series.db_id is not None:
             return False
 
         quality_profile_id = self._get_quality_profile_id(profile)
+        language_profile_id = self._sonarr.get_language_profile()[0]["id"]
+        root_folder = self._sonarr.get_root_folder()
+        assert isinstance(root_folder, list)
+        root_folder_path = root_folder[0]["path"]
 
-        root_folder = cast(list[json], self._radarr.get_root_folder())[0]["path"]
-
-        self._radarr.add_movie(
-            db_id=movie.tmdb_id,
+        series_json = self._sonarr.add_series(
+            series._json,
             quality_profile_id=quality_profile_id,
-            root_dir=root_folder,
+            language_profile_id=language_profile_id,
+            root_dir=root_folder_path,
+            search_for_missing_episodes=True,
         )
 
-        return True
-
-    def del_movie(self, movie: Movie) -> None:
-        potential = cast(list[json], self._radarr.get_movie(movie.tmdb_id))
+        series.db_id = series_json["id"]
 
-        if not potential:
-            raise ValueError(f"{movie} is not in the library")
+        return True
 
-        movie_json = potential[0]
+    def del_series(self, series: Series) -> None:
+        if series.db_id is None:
+            raise ValueError(f"{series} is not in the library")
 
-        db_id = movie_json["id"]
-        path = movie_json["folderName"]
+        series_json = self._sonarr.get_series(series.db_id)
+        assert isinstance(series_json, dict)
 
-        self._radarr.del_movie(db_id, delete_files=True, add_exclusion=False)
+        self._sonarr.del_series(series.db_id, delete_files=True)
 
         try:
-            rmtree(path)
+            rmtree(series_json["path"])
         except FileNotFoundError:
             pass
 
-    def movie_downloaded(self, movie: Movie) -> bool:
-        potential = cast(list[json], self._radarr.get_movie(movie.tmdb_id))
-
-        if not potential:
+    def series_downloaded(self, series: Series) -> bool:
+        if series.db_id is None:
             return False
 
-        files = self._radarr.get_movie_files_by_movie_id(potential[0]["id"])
+        files = self._sonarr.get_episode_files_by_series_id(series.db_id)
 
         if files:
             return True
 
         return False
 
     def create_tag(self, tag: str) -> None:
-        self._radarr.create_tag(tag)
-
-    def add_tag(self, movie: Movie | list[Movie], user_id: int) -> bool:
-        if isinstance(movie, Movie):
-            ids = [cast(list[json], self._radarr.get_movie(movie.tmdb_id))[0]["id"]]
-        else:
-            ids = [
-                cast(list[json], self._radarr.get_movie(m.tmdb_id))[0]["id"]
-                for m in movie
-            ]
+        self._sonarr.create_tag(tag)
 
+    def add_tag(self, series: Series, user_id: int) -> bool:
         try:
             tag_id = self._get_tag_for_user_id(user_id)
         except ValueError:
             # tag_id = self._radarr.create_tag(str(user_id))['id']
 
             return False
 
-        edit_json = {"movieIds": ids, "tags": [tag_id], "applyTags": "add"}
+        series_json = self._sonarr.get_series(series.db_id)
+        assert isinstance(series_json, dict)
+
+        series_json["tags"].append(tag_id)
 
-        self._radarr.upd_movies(edit_json)
+        self._sonarr.upd_series(series_json)
 
         return True
 
     def get_downloads(self) -> list[Download]:
-        queue = cast(list[json], self._radarr.get_queue_details())
+        queue = self._sonarr.get_queue()["records"]
 
         downloads = [Download(d) for d in queue]
 
-        return sorted(downloads, key=lambda d: (d.timeleft, -d.pct_done))
+        return downloads
 
     def get_quota_amount(self, user_id: int) -> int:
         try:
             tag_id = self._get_tag_for_user_id(user_id)
         except ValueError:
             return 0
 
         total = 0
 
-        for movie in cast(list[json], self._radarr.get_movie()):
-            if tag_id in movie["tags"]:
-                total += movie["sizeOnDisk"]
+        for series in self._sonarr.get_series():
+            assert isinstance(series, dict)
+            if tag_id in series["tags"]:
+                total += series["statistics"]["sizeOnDisk"]
 
         return total
 
     def get_quality_profile_name(self, profile_id: int) -> str:
-        profiles = cast(list[json], self._radarr.get_quality_profile())
+        profiles = self._sonarr.get_quality_profile()
 
         for profile in profiles:
             if profile["id"] == profile_id:
-                return cast(str, profile["name"])
+                name = profile["name"]
+                assert isinstance(name, str)
+                return name
 
         raise ValueError(f"no quality profile with the id {profile_id}")
 
-    def rescan_movie(self, movie_id: int) -> None:
-        self._radarr.post_command("RescanMovie", movieId=movie_id)
-
-    def refresh_movie(self, movie_id: int) -> None:
-        self._radarr.post_command("RefreshMovie", movieIds=[movie_id])
-
-    def search_missing(self) -> None:
-        self._radarr.post_command(name="MissingMoviesSearch")
+    def rescan_series(self, series_id: int) -> None:
+        self._sonarr.post_command("RescanSeries", seriesId=series_id)  # type: ignore
 
     def _get_quality_profile_id(self, name: str) -> int:
-        profiles = cast(list[json], self._radarr.get_quality_profile())
+        profiles = self._sonarr.get_quality_profile()
 
         for profile in profiles:
             if profile["name"].lower() == name.lower():
-                return cast(int, profile["id"])
+                profile_id = profile["id"]
+                assert isinstance(profile_id, int)
+                return profile_id
 
         raise ValueError(f"no quality profile with the name {name}")
 
     def _get_tag_for_user_id(self, user_id: int) -> int:
-        tags = cast(list[json], self._radarr.get_tag())
+        tags = self._sonarr.get_tag()
+        assert isinstance(tags, list)
 
         for tag in tags:
             if str(user_id) in tag["label"]:
-                return cast(int, tag["id"])
+                tag_id = tag["id"]
+                assert isinstance(tag_id, int)
+                return tag_id
 
         raise ValueError(f"no tag with the user id {user_id}")
-
-
-__all__ = ["Movie"]
-
-
-if __name__ == "__main__":
-    from wi1_bot.config import config
-
-    radarr = Radarr(config["radarr"]["url"], config["radarr"]["api_key"])
-    pyarr = radarr._radarr
```

### Comparing `wi1-bot-1.3.5/wi1_bot/arr/sonarr.py` & `wi1-bot-1.3.6/wi1_bot/arr/radarr.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,192 +1,191 @@
 from shutil import rmtree
-from typing import Any, cast
 
-from pyarr import SonarrAPI
+from pyarr import RadarrAPI
 
 from .download import Download
+from .movie import Movie
 
-json = dict[str, Any]
 
-
-class Series:
-    def __init__(self, series_json: dict[str, Any]) -> None:
-        self.title: str = series_json["title"]
-        self.year: int = series_json["year"]
-        self.tvdb_id: int = series_json["tvdbId"]
-
-        self.db_id: int | None = series_json["id"] if "id" in series_json else None
-
-        self.full_title = f"{self.title} ({self.year})"
-
-        self.url = f"https://thetvdb.com/dereferrer/series/{self.tvdb_id}"
-
-        self.imdb_id = ""
-
-        try:
-            self.imdb_id = series_json["imdbId"]
-            self.url = f"https://imdb.com/title/{self.imdb_id}"
-        except KeyError:
-            pass
-
-    def __str__(self) -> str:
-        return f"[{self.full_title}]({self.url})"
-
-    def __repr__(self) -> str:
-        return str(self.__dict__)
-
-
-class SonarrError(Exception):
-    pass
-
-
-class Sonarr:
+class Radarr:
     def __init__(self, url: str, api_key: str) -> None:
-        self._sonarr = SonarrAPI(url, api_key)
-
-    def lookup_series(self, query: str) -> list[Series]:
-        possible_series = cast(
-            list[json] | dict[str, Any], self._sonarr.lookup_series(query)
-        )
+        self._radarr = RadarrAPI(url, api_key)
 
-        if isinstance(possible_series, dict):
-            raise SonarrError(possible_series["message"])
+    def lookup_movie(self, query: str) -> list[Movie]:
+        possible_movies = self._radarr.lookup_movie(query)
 
-        return [Series(s) for s in possible_series]
+        return [Movie(m) for m in possible_movies]
 
-    def lookup_library(self, query: str) -> list[Series]:
-        possible_series = cast(list[json], self._sonarr.lookup_series(query))
+    def lookup_library(self, query: str) -> list[Movie]:
+        possible_movies = self._radarr.lookup_movie(query)
 
-        return [Series(s) for s in possible_series if "id" in s]
+        return [Movie(m) for m in possible_movies if "id" in m]
 
-    def lookup_user_library(self, query: str, user_id: int) -> list[Series]:
+    def lookup_user_library(self, query: str, user_id: int) -> list[Movie]:
         try:
             tag_id = self._get_tag_for_user_id(user_id)
         except ValueError:
             return []
 
-        possible_series = cast(list[json], self._sonarr.lookup_series(query))
+        tag_detail = self._radarr.get_tag_detail(tag_id)
+        assert isinstance(tag_detail, dict)
+
+        possible_movies = self._radarr.lookup_movie(query)
 
-        # self._sonarr.get_tag_detail is broken/not supported in v1 sonarr API so have
-        # to filter the tmdb lookup (probably slower but saves an API call)
-        user_series = [s for s in possible_series if tag_id in s["tags"]]
+        user_movie_ids = tag_detail["movieIds"]
 
-        return [Series(s) for s in user_series]
+        return [
+            Movie(m) for m in possible_movies if "id" in m and m["id"] in user_movie_ids
+        ]
 
-    def add_series(self, series: Series, profile: str = "good") -> bool:
-        if series.db_id is not None:
+    def add_movie(self, movie: Movie, profile: str = "good") -> bool:
+        if self._radarr.get_movie(movie.tmdb_id, tmdb=True):
             return False
 
         quality_profile_id = self._get_quality_profile_id(profile)
 
-        root_folder = cast(list[json], self._sonarr.get_root_folder())[0]["path"]
-
-        series_json = cast(
-            json,
-            self._sonarr.add_series(
-                tvdb_id=series.tvdb_id,
-                quality_profile_id=quality_profile_id,
-                root_dir=root_folder,
-                search_for_missing_episodes=True,
-            ),
+        root_folder = self._radarr.get_root_folder()
+        assert isinstance(root_folder, list)
+        root_folder_path = root_folder[0]["path"]
+
+        self._radarr.add_movie(
+            movie._json,
+            root_dir=root_folder_path,
+            quality_profile_id=quality_profile_id,
         )
 
-        series.db_id = series_json["id"]
-
         return True
 
-    def del_series(self, series: Series) -> None:
-        if series.db_id is None:
-            raise ValueError(f"{series} is not in the library")
+    def del_movie(self, movie: Movie) -> None:
+        potential = self._radarr.get_movie(movie.tmdb_id, tmdb=True)
+        assert isinstance(potential, list)
+
+        if not potential:
+            raise ValueError(f"{movie} is not in the library")
+
+        movie_json = potential[0]
 
-        series_json = cast(json, self._sonarr.get_series(series.db_id))
+        db_id = movie_json["id"]
+        path = movie_json["folderName"]
 
-        self._sonarr.del_series(series.db_id, delete_files=True)
+        self._radarr.del_movie(db_id, delete_files=True, add_exclusion=False)
 
         try:
-            rmtree(series_json["path"])
+            rmtree(path)
         except FileNotFoundError:
             pass
 
-    def series_downloaded(self, series: Series) -> bool:
-        if series.db_id is None:
-            return False
+    def movie_downloaded(self, movie: Movie) -> bool:
+        potential = self._radarr.get_movie(movie.tmdb_id, tmdb=True)
+        assert isinstance(potential, list)
 
-        files = self._sonarr.get_episode_files_by_series_id(series.db_id)
+        if not potential:
+            return False
 
-        if files:
-            return True
+        files = self._radarr.get_movie_files_by_movie_id(potential[0]["id"])
 
-        return False
+        return len(files) > 0
 
     def create_tag(self, tag: str) -> None:
-        self._sonarr.create_tag(tag)
+        self._radarr.create_tag(tag)
+
+    def add_tag(self, movie: Movie | list[Movie], user_id: int) -> bool:
+        if isinstance(movie, Movie):
+            json = self._radarr.get_movie(movie.tmdb_id, tmdb=True)
+            assert isinstance(json, list)
+            ids = [json[0]["id"]]
+        else:
+            ids = []
+
+            for m in movie:
+                json = self._radarr.get_movie(m.tmdb_id, tmdb=True)
+                assert isinstance(json, list)
+                ids.append(json[0]["id"])
 
-    def add_tag(self, series: Series, user_id: int) -> bool:
         try:
             tag_id = self._get_tag_for_user_id(user_id)
         except ValueError:
             # tag_id = self._radarr.create_tag(str(user_id))['id']
 
             return False
 
-        series_json = cast(json, self._sonarr.get_series(series.db_id))
-
-        series_json["tags"].append(tag_id)
+        edit_json = {"movieIds": ids, "tags": [tag_id], "applyTags": "add"}
 
-        self._sonarr.upd_series(series_json)
+        self._radarr.upd_movies(edit_json)
 
         return True
 
     def get_downloads(self) -> list[Download]:
-        queue = cast(list[json], self._sonarr.get_queue())
+        queue = self._radarr.get_queue_details()
 
         downloads = [Download(d) for d in queue]
 
-        return downloads
+        return sorted(downloads, key=lambda d: (d.timeleft, -d.pct_done))
 
     def get_quota_amount(self, user_id: int) -> int:
         try:
             tag_id = self._get_tag_for_user_id(user_id)
         except ValueError:
             return 0
 
         total = 0
 
-        for series in cast(list[json], self._sonarr.get_series()):
-            if tag_id in series["tags"]:
-                try:
-                    total += series["sizeOnDisk"]
-                except KeyError:
-                    continue
+        for movie in self._radarr.get_movie():
+            assert isinstance(movie, dict)
+
+            if tag_id in movie["tags"]:
+                total += movie["sizeOnDisk"]
 
         return total
 
     def get_quality_profile_name(self, profile_id: int) -> str:
-        profiles = cast(list[json], self._sonarr.get_quality_profile())
+        profiles = self._radarr.get_quality_profile()
 
         for profile in profiles:
             if profile["id"] == profile_id:
-                return cast(str, profile["name"])
+                name = profile["name"]
+                assert isinstance(name, str)
+                return name
 
         raise ValueError(f"no quality profile with the id {profile_id}")
 
-    def rescan_series(self, series_id: int) -> None:
-        self._sonarr.post_command("RescanSeries", seriesId=series_id)
+    def rescan_movie(self, movie_id: int) -> None:
+        self._radarr.post_command("RescanMovie", movieId=movie_id)  # type: ignore
+
+    def refresh_movie(self, movie_id: int) -> None:
+        self._radarr.post_command("RefreshMovie", movieIds=[movie_id])  # type: ignore
+
+    def search_missing(self) -> None:
+        self._radarr.post_command(name="MissingMoviesSearch")
 
     def _get_quality_profile_id(self, name: str) -> int:
-        profiles = cast(list[json], self._sonarr.get_quality_profile())
+        profiles = self._radarr.get_quality_profile()
 
         for profile in profiles:
             if profile["name"].lower() == name.lower():
-                return cast(int, profile["id"])
+                profile_id = profile["id"]
+                assert isinstance(profile_id, int)
+                return profile_id
 
         raise ValueError(f"no quality profile with the name {name}")
 
     def _get_tag_for_user_id(self, user_id: int) -> int:
-        tags = cast(list[json], self._sonarr.get_tag())
+        tags = self._radarr.get_tag()
+        assert isinstance(tags, list)
 
         for tag in tags:
             if str(user_id) in tag["label"]:
-                return cast(int, tag["id"])
+                tag_id = tag["id"]
+                assert isinstance(tag_id, int)
+                return tag_id
 
         raise ValueError(f"no tag with the user id {user_id}")
+
+
+__all__ = ["Movie"]
+
+
+if __name__ == "__main__":
+    from wi1_bot.config import config
+
+    radarr = Radarr(config["radarr"]["url"], config["radarr"]["api_key"])
+    pyarr = radarr._radarr
```

### Comparing `wi1-bot-1.3.5/wi1_bot/config.py` & `wi1-bot-1.3.6/wi1_bot/config.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.5/wi1_bot/discord/bot.py` & `wi1-bot-1.3.6/wi1_bot/discord/bot.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.5/wi1_bot/discord/cogs/movie.py` & `wi1-bot-1.3.6/wi1_bot/discord/cogs/movie.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.5/wi1_bot/discord/cogs/series.py` & `wi1-bot-1.3.6/wi1_bot/discord/cogs/series.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.5/wi1_bot/discord/helpers.py` & `wi1-bot-1.3.6/wi1_bot/discord/helpers.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.5/wi1_bot/push.py` & `wi1-bot-1.3.6/wi1_bot/push.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.5/wi1_bot/scripts/add_tag.py` & `wi1-bot-1.3.6/wi1_bot/scripts/add_tag.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.5/wi1_bot/scripts/start.py` & `wi1-bot-1.3.6/wi1_bot/scripts/start.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.5/wi1_bot/scripts/transcode_item.py` & `wi1-bot-1.3.6/wi1_bot/scripts/transcode_item.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.5/wi1_bot/transcoder/transcode_queue.py` & `wi1-bot-1.3.6/wi1_bot/transcoder/transcode_queue.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.5/wi1_bot/transcoder/transcoder.py` & `wi1-bot-1.3.6/wi1_bot/transcoder/transcoder.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.3.5/wi1_bot/webhook.py` & `wi1-bot-1.3.6/wi1_bot/webhook.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import json
 import logging
 import os.path
 import threading
-from typing import Any, cast
+from typing import Any
 
 from flask import Flask, request
 
 from wi1_bot import push, transcoder
 from wi1_bot.arr import Radarr, Sonarr
 from wi1_bot.config import config
 
@@ -24,34 +25,34 @@
         req["release"]["releaseTitle"], title=f"file grabbed ({req['downloadClient']})"
     )
 
 
 def on_download(req: dict[str, Any]) -> None:
     if "movie" in req:
         content_id = req["movie"]["id"]
+        movie_json = radarr._radarr.get_movie(content_id)
+        assert isinstance(movie_json, dict)
 
         quality_profile = radarr.get_quality_profile_name(
-            cast(dict[str, Any], radarr._radarr.get_movie_by_movie_id(content_id))[
-                "qualityProfileId"
-            ]
+            movie_json["qualityProfileId"]
         )
 
         movie_folder = req["movie"]["folderPath"]
         basename = req["movieFile"]["relativePath"]
 
         push.send(basename, title="movie downloaded")
 
         path = os.path.join(movie_folder, basename)
     elif "series" in req:
         content_id = req["series"]["id"]
+        series_json = sonarr._sonarr.get_series(content_id)
+        assert isinstance(series_json, dict)
 
         quality_profile = sonarr.get_quality_profile_name(
-            cast(dict[str, Any], sonarr._sonarr.get_series(content_id))[
-                "qualityProfileId"
-            ]
+            series_json["qualityProfileId"]
         )
 
         series_folder = req["series"]["path"]
         relative_path = req["episodeFile"]["relativePath"]
 
         push.send(relative_path.split("/")[-1], title="episode downloaded")
 
@@ -93,15 +94,15 @@
 
 @app.route("/", methods=["POST"])
 def index() -> Any:
     try:
         if request.json is None or "eventType" not in request.json:
             return "", 400
 
-        logger.debug(f"got request: {request.json}")
+        logger.debug(f"got request: {json.dumps(request.json, indent=4)}")
 
         if request.json["eventType"] == "Grab":
             on_grab(request.json)
         elif request.json["eventType"] == "Download":
             on_download(request.json)
     except Exception:
         logger.warning(
```

### Comparing `wi1-bot-1.3.5/wi1_bot.egg-info/PKG-INFO` & `wi1-bot-1.3.6/wi1_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wi1-bot
-Version: 1.3.5
+Version: 1.3.6
 Summary: Discord bot for Radarr/Sonarr integration
 Home-page: https://github.com/wthueb/wi1-bot
 Author-email: William Huebner <wilhueb@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 William Huebner
```

### Comparing `wi1-bot-1.3.5/wi1_bot.egg-info/SOURCES.txt` & `wi1-bot-1.3.6/wi1_bot.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 .pre-commit-config.yaml
 LICENSE
 README.md
 config.yaml.template
 pyproject.toml
 setup.cfg
 .github/workflows/pypi-publish.yml
+.vscode/launch.json
+.vscode/settings.json
 tests/movie_downloaded.py
 wi1_bot/__init__.py
 wi1_bot/_version.py
 wi1_bot/config.py
 wi1_bot/push.py
 wi1_bot/webhook.py
 wi1_bot.egg-info/PKG-INFO
```

