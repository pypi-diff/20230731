# Comparing `tmp/mov_cli-1.5.0.tar.gz` & `tmp/mov_cli-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli-1.5.0.tar", max compression
+gzip compressed data, was "mov_cli-1.5.1.tar", max compression
```

## Comparing `mov_cli-1.5.0.tar` & `mov_cli-1.5.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0    35149 2023-07-29 02:41:41.922399 mov_cli-1.5.0/LICENSE
--rw-r--r--   0        0        0     6568 2023-07-29 02:41:41.922399 mov_cli-1.5.0/README.md
--rw-r--r--   0        0        0      657 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/__init__.py
--rw-r--r--   0        0        0      810 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/__main__.py
--rw-r--r--   0        0        0        1 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/extractors/__init__.py
--rw-r--r--   0        0        0      906 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/extractors/doodstream.py
--rw-r--r--   0        0        0       71 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/extractors/scdn/NOTICE
--rw-r--r--   0        0        0        1 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/extractors/scdn/__init__.py
--rw-r--r--   0        0        0      169 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/extractors/scdn/allsportsdaily.py
--rw-r--r--   0        0        0      958 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/extractors/scdn/cr7sports.py
--rw-r--r--   0        0        0      256 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/extractors/scdn/enjoy4hd.py
--rw-r--r--   0        0        0      141 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/extractors/scdn/fabtech.py
--rw-r--r--   0        0        0      218 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/extractors/scdn/gameshdlive.py
--rw-r--r--   0        0        0      457 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/extractors/scdn/livestreames.py
--rw-r--r--   0        0        0      318 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/extractors/scdn/methstreams.py
--rw-r--r--   0        0        0      156 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/extractors/scdn/motornews.py
--rw-r--r--   0        0        0      873 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/extractors/scdn/onestream.py
--rw-r--r--   0        0        0      891 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/extractors/scdn/onionlive.py
--rw-r--r--   0        0        0      615 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/extractors/scdn/onionstream.py
--rw-r--r--   0        0        0      457 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/extractors/scdn/poscitech.py
--rw-r--r--   0        0        0      638 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/extractors/scdn/rainostreams.py
--rw-r--r--   0        0        0      358 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/extractors/scdn/ripple.py
--rw-r--r--   0        0        0      406 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/extractors/scdn/techclips.py
--rw-r--r--   0        0        0      417 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/extractors/scdn/techstips.py
--rw-r--r--   0        0        0     1333 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/extractors/scdn/weakstream.py
--rw-r--r--   0        0        0      341 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/extractors/tukipasti.py
--rw-r--r--   0        0        0        0 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/players/__init__.py
--rw-r--r--   0        0        0     3128 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/players/player.py
--rw-r--r--   0        0        0        0 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/utils/__init__.py
--rw-r--r--   0        0        0     2772 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/utils/httpclient.py
--rw-r--r--   0        0        0      356 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/utils/lang/ar.json
--rw-r--r--   0        0        0      356 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/utils/lang/de.json
--rw-r--r--   0        0        0      309 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/utils/lang/en.json
--rw-r--r--   0        0        0      348 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/utils/lang/fr.json
--rw-r--r--   0        0        0      338 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/utils/lang/ko.json
--rw-r--r--   0        0        0      194 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/utils/lang/langs
--rw-r--r--   0        0        0      308 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/utils/lang/pl.json
--rw-r--r--   0        0        0      289 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/utils/lang/pt.json
--rw-r--r--   0        0        0      418 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/utils/lang/ru.json
--rw-r--r--   0        0        0      660 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/utils/lang/ta.json
--rw-r--r--   0        0        0     1258 2023-07-29 02:41:41.922399 mov_cli-1.5.0/mov_cli/utils/lang.py
--rw-r--r--   0        0        0     1570 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/utils/player.py
--rw-r--r--   0        0        0     1505 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/utils/props.py
--rw-r--r--   0        0        0     7437 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/utils/scraper.py
--rw-r--r--   0        0        0     5058 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/utils/select.py
--rw-r--r--   0        0        0        0 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/anime/__init__.py
--rw-r--r--   0        0        0     3274 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/anime/gogoanime.py
--rw-r--r--   0        0        0        0 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/asian/__init__.py
--rw-r--r--   0        0        0     3755 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/asian/viewasian.py
--rw-r--r--   0        0        0     3382 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/asian/watchasian.py
--rw-r--r--   0        0        0        0 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/cartoons/__init__.py
--rw-r--r--   0        0        0     3544 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/cartoons/kisscartoon.py
--rw-r--r--   0        0        0        0 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/english/__init__.py
--rw-r--r--   0        0        0     7686 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/english/actvid.py
--rw-r--r--   0        0        0     3843 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/english/dopebox.py
--rw-r--r--   0        0        0     4242 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/english/remotestream.py
--rw-r--r--   0        0        0     3847 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/english/sflix.py
--rw-r--r--   0        0        0     1626 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/english/solar.py
--rw-r--r--   0        0        0        0 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/indian/__init__.py
--rw-r--r--   0        0        0     1943 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/indian/einthusan.py
--rw-r--r--   0        0        0     2165 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/indian/streamblasters.py
--rw-r--r--   0        0        0     1358 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/indian/tamilyogi.py
--rw-r--r--   0        0        0        0 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/international/__init__.py
--rw-r--r--   0        0        0     3950 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/international/wlext.py
--rw-r--r--   0        0        0        0 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/livetv/__init__.py
--rw-r--r--   0        0        0     1559 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/livetv/eja.py
--rw-r--r--   0        0        0        0 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/sports/__init__.py
--rw-r--r--   0        0        0     4474 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/sports/scdn.py
--rw-r--r--   0        0        0        0 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/turkish/__init__.py
--rw-r--r--   0        0        0     2318 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/turkish/turkish123.py
--rw-r--r--   0        0        0     2909 2023-07-29 02:41:41.926399 mov_cli-1.5.0/mov_cli/websites/turkish/yoturkish.py
--rw-r--r--   0        0        0      736 2023-07-29 02:41:41.926399 mov_cli-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     7557 1970-01-01 00:00:00.000000 mov_cli-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-31 06:44:15.639737 mov_cli-1.5.1/LICENSE
+-rw-r--r--   0        0        0     6568 2023-07-31 06:44:15.639737 mov_cli-1.5.1/README.md
+-rw-r--r--   0        0        0      657 2023-07-31 06:44:15.639737 mov_cli-1.5.1/mov_cli/__init__.py
+-rw-r--r--   0        0        0      810 2023-07-31 06:44:15.639737 mov_cli-1.5.1/mov_cli/__main__.py
+-rw-r--r--   0        0        0        1 2023-07-31 06:44:15.639737 mov_cli-1.5.1/mov_cli/extractors/__init__.py
+-rw-r--r--   0        0        0      906 2023-07-31 06:44:15.639737 mov_cli-1.5.1/mov_cli/extractors/doodstream.py
+-rw-r--r--   0        0        0       71 2023-07-31 06:44:15.639737 mov_cli-1.5.1/mov_cli/extractors/scdn/NOTICE
+-rw-r--r--   0        0        0        1 2023-07-31 06:44:15.639737 mov_cli-1.5.1/mov_cli/extractors/scdn/__init__.py
+-rw-r--r--   0        0        0      169 2023-07-31 06:44:15.639737 mov_cli-1.5.1/mov_cli/extractors/scdn/allsportsdaily.py
+-rw-r--r--   0        0        0      958 2023-07-31 06:44:15.639737 mov_cli-1.5.1/mov_cli/extractors/scdn/cr7sports.py
+-rw-r--r--   0        0        0      256 2023-07-31 06:44:15.639737 mov_cli-1.5.1/mov_cli/extractors/scdn/enjoy4hd.py
+-rw-r--r--   0        0        0      141 2023-07-31 06:44:15.639737 mov_cli-1.5.1/mov_cli/extractors/scdn/fabtech.py
+-rw-r--r--   0        0        0      218 2023-07-31 06:44:15.639737 mov_cli-1.5.1/mov_cli/extractors/scdn/gameshdlive.py
+-rw-r--r--   0        0        0      457 2023-07-31 06:44:15.639737 mov_cli-1.5.1/mov_cli/extractors/scdn/livestreames.py
+-rw-r--r--   0        0        0      318 2023-07-31 06:44:15.639737 mov_cli-1.5.1/mov_cli/extractors/scdn/methstreams.py
+-rw-r--r--   0        0        0      156 2023-07-31 06:44:15.639737 mov_cli-1.5.1/mov_cli/extractors/scdn/motornews.py
+-rw-r--r--   0        0        0      873 2023-07-31 06:44:15.639737 mov_cli-1.5.1/mov_cli/extractors/scdn/onestream.py
+-rw-r--r--   0        0        0      891 2023-07-31 06:44:15.639737 mov_cli-1.5.1/mov_cli/extractors/scdn/onionlive.py
+-rw-r--r--   0        0        0      615 2023-07-31 06:44:15.639737 mov_cli-1.5.1/mov_cli/extractors/scdn/onionstream.py
+-rw-r--r--   0        0        0      457 2023-07-31 06:44:15.639737 mov_cli-1.5.1/mov_cli/extractors/scdn/poscitech.py
+-rw-r--r--   0        0        0      638 2023-07-31 06:44:15.639737 mov_cli-1.5.1/mov_cli/extractors/scdn/rainostreams.py
+-rw-r--r--   0        0        0      358 2023-07-31 06:44:15.639737 mov_cli-1.5.1/mov_cli/extractors/scdn/ripple.py
+-rw-r--r--   0        0        0      406 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/extractors/scdn/techclips.py
+-rw-r--r--   0        0        0      417 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/extractors/scdn/techstips.py
+-rw-r--r--   0        0        0     1333 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/extractors/scdn/weakstream.py
+-rw-r--r--   0        0        0      341 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/extractors/tukipasti.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/players/__init__.py
+-rw-r--r--   0        0        0     3128 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/players/player.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/utils/__init__.py
+-rw-r--r--   0        0        0     2772 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/utils/httpclient.py
+-rw-r--r--   0        0        0      356 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/utils/lang/ar.json
+-rw-r--r--   0        0        0      356 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/utils/lang/de.json
+-rw-r--r--   0        0        0      309 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/utils/lang/en.json
+-rw-r--r--   0        0        0      348 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/utils/lang/fr.json
+-rw-r--r--   0        0        0      338 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/utils/lang/ko.json
+-rw-r--r--   0        0        0      194 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/utils/lang/langs
+-rw-r--r--   0        0        0      308 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/utils/lang/pl.json
+-rw-r--r--   0        0        0      289 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/utils/lang/pt.json
+-rw-r--r--   0        0        0      418 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/utils/lang/ru.json
+-rw-r--r--   0        0        0      660 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/utils/lang/ta.json
+-rw-r--r--   0        0        0     1258 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/utils/lang.py
+-rw-r--r--   0        0        0     1570 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/utils/player.py
+-rw-r--r--   0        0        0     1505 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/utils/props.py
+-rw-r--r--   0        0        0     7437 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/utils/scraper.py
+-rw-r--r--   0        0        0     5058 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/utils/select.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/anime/__init__.py
+-rw-r--r--   0        0        0     3274 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/anime/gogoanime.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/asian/__init__.py
+-rw-r--r--   0        0        0     3755 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/asian/viewasian.py
+-rw-r--r--   0        0        0     3382 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/asian/watchasian.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/cartoons/__init__.py
+-rw-r--r--   0        0        0     3544 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/cartoons/kisscartoon.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/english/__init__.py
+-rw-r--r--   0        0        0     7787 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/english/actvid.py
+-rw-r--r--   0        0        0     3861 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/english/dopebox.py
+-rw-r--r--   0        0        0     4242 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/english/remotestream.py
+-rw-r--r--   0        0        0     3865 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/english/sflix.py
+-rw-r--r--   0        0        0     1638 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/english/solar.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/indian/__init__.py
+-rw-r--r--   0        0        0     1943 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/indian/einthusan.py
+-rw-r--r--   0        0        0     2165 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/indian/streamblasters.py
+-rw-r--r--   0        0        0     1358 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/indian/tamilyogi.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/international/__init__.py
+-rw-r--r--   0        0        0     3950 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/international/wlext.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/livetv/__init__.py
+-rw-r--r--   0        0        0     1559 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/livetv/eja.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/sports/__init__.py
+-rw-r--r--   0        0        0     4474 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/sports/scdn.py
+-rw-r--r--   0        0        0        0 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/turkish/__init__.py
+-rw-r--r--   0        0        0     2318 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/turkish/turkish123.py
+-rw-r--r--   0        0        0     2909 2023-07-31 06:44:15.643737 mov_cli-1.5.1/mov_cli/websites/turkish/yoturkish.py
+-rw-r--r--   0        0        0      737 2023-07-31 06:44:15.643737 mov_cli-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     7557 1970-01-01 00:00:00.000000 mov_cli-1.5.1/PKG-INFO
```

### Comparing `mov_cli-1.5.0/LICENSE` & `mov_cli-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/README.md` & `mov_cli-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/__init__.py` & `mov_cli-1.5.1/mov_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/__main__.py` & `mov_cli-1.5.1/mov_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/extractors/doodstream.py` & `mov_cli-1.5.1/mov_cli/extractors/doodstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/extractors/scdn/cr7sports.py` & `mov_cli-1.5.1/mov_cli/extractors/scdn/cr7sports.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/extractors/scdn/onestream.py` & `mov_cli-1.5.1/mov_cli/extractors/scdn/onestream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/extractors/scdn/onionlive.py` & `mov_cli-1.5.1/mov_cli/extractors/scdn/onionlive.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/extractors/scdn/onionstream.py` & `mov_cli-1.5.1/mov_cli/extractors/scdn/onionstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/extractors/scdn/rainostreams.py` & `mov_cli-1.5.1/mov_cli/extractors/scdn/rainostreams.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/extractors/scdn/weakstream.py` & `mov_cli-1.5.1/mov_cli/extractors/scdn/weakstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/players/player.py` & `mov_cli-1.5.1/mov_cli/players/player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/utils/httpclient.py` & `mov_cli-1.5.1/mov_cli/utils/httpclient.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/utils/lang/ta.json` & `mov_cli-1.5.1/mov_cli/utils/lang/ta.json`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/utils/lang.py` & `mov_cli-1.5.1/mov_cli/utils/lang.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/utils/player.py` & `mov_cli-1.5.1/mov_cli/utils/player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/utils/props.py` & `mov_cli-1.5.1/mov_cli/utils/props.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/utils/scraper.py` & `mov_cli-1.5.1/mov_cli/utils/scraper.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/utils/select.py` & `mov_cli-1.5.1/mov_cli/utils/select.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/websites/anime/gogoanime.py` & `mov_cli-1.5.1/mov_cli/websites/anime/gogoanime.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/websites/asian/viewasian.py` & `mov_cli-1.5.1/mov_cli/websites/asian/viewasian.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/websites/asian/watchasian.py` & `mov_cli-1.5.1/mov_cli/websites/asian/watchasian.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/websites/cartoons/kisscartoon.py` & `mov_cli-1.5.1/mov_cli/websites/cartoons/kisscartoon.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/websites/english/actvid.py` & `mov_cli-1.5.1/mov_cli/websites/english/actvid.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,20 @@
                 "embed-1", "embed-1/ajax/e-1/"
             ),
             parts[-1],
         )
 
     ## Decrypting the sources
 
+    def is_base64(self, s):
+        try:
+            base64.b64encode(s)
+        except Exception:
+            return False
+
     def repair_base64(self, s):
         missing_padding = len(s) % 4
         if missing_padding != 0:
             s += '=' * (4 - missing_padding)
         return s
 
     def gh_key(self):
@@ -111,17 +117,16 @@
             x = self.md5(x + key + salt)
             currentkey += x
         return currentkey
     
     def decrypt_aes(self, encrypted_data, key):
         dec_key = key[:32]
         iv = key[32:]
-        print(iv, dec_key)
         cipher = AES.new(dec_key, AES.MODE_CBC, iv=iv)
-        decrypted_data = unpad(cipher.decrypt(encrypted_data[16:]), AES.block_size)
+        decrypted_data = unpad(cipher.decrypt(encrypted_data[16:]), cipher.block_size)
         return decrypted_data.decode('utf-8')
 
     def decrypt(self, data, key): # dokicloud = pain :'(
         data = self.repair_base64(data)
         sources_array = list(data)
         extracted_key = ""
```

### Comparing `mov_cli-1.5.0/mov_cli/websites/english/dopebox.py` & `mov_cli-1.5.1/mov_cli/websites/english/dopebox.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .actvid import Provider as pv
 from bs4 import BeautifulSoup as BS
 from urllib import parse as p
 import re
+import json
 
 class Provider(pv):
     def __init__(self, base_url) -> None:
         super().__init__(base_url)
         self.base_url = base_url
         self.dseasonp = True
         self.dshowp = True
@@ -32,15 +33,15 @@
             ),
             parts[-1],
         )
 
     def gh_key(self):
         response_key = self.client.get('https://github.com/enimax-anime/key/blob/e4/key.txt').json()
         key = response_key["payload"]["blob"]["rawLines"][0]
-        key = eval(key)
+        key = json.loads(key)
         return key
 
     def server_id(self, mov_id):
         rem = self.client.get(f"{self.base_url}/ajax/movie/episodes/{mov_id}")
         soup = BS(rem, self.scraper)
         return [i["data-id"] for i in soup.select(".link-item")][0]
```

### Comparing `mov_cli-1.5.0/mov_cli/websites/english/remotestream.py` & `mov_cli-1.5.1/mov_cli/websites/english/remotestream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/websites/english/sflix.py` & `mov_cli-1.5.1/mov_cli/websites/english/sflix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .actvid import Provider as pv
 from bs4 import BeautifulSoup as BS
 from urllib import parse as p
 import re
+import json
 
 class Provider(pv):
     def __init__(self, base_url) -> None:
         super().__init__(base_url)
         self.base_url = base_url
         self.dseasonp = True
         self.dshowp = True
@@ -37,15 +38,15 @@
             ),
             parts[-1],
         )
 
     def gh_key(self):
         response_key = self.client.get('https://github.com/enimax-anime/key/blob/e4/key.txt').json()
         key = response_key["payload"]["blob"]["rawLines"][0]
-        key = eval(key)
+        key = json.loads(key)
         return key
 
     def server_id(self, mov_id):
         rem = self.client.get(f"{self.base_url}/ajax/movie/episodes/{mov_id}")
         soup = BS(rem, self.scraper)
         return [i["data-id"] for i in soup.select(".link-item")][0]
```

### Comparing `mov_cli-1.5.0/mov_cli/websites/english/solar.py` & `mov_cli-1.5.1/mov_cli/websites/english/solar.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .actvid import Provider as pv
 from bs4 import BeautifulSoup as BS
 from urllib import parse as p
-import re
+import re, json
 
 class Provider(pv):
     def __init__(self, base_url) -> None:
         super().__init__(base_url)
         self.base_url = base_url
         self.dseasonp = True
         self.dshowp = True
@@ -32,15 +32,15 @@
             ),
             parts[-1],
         )
 
     def gh_key(self):
         response_key = self.client.get('https://github.com/enimax-anime/key/blob/e4/key.txt').json()
         key = response_key["payload"]["blob"]["rawLines"][0]
-        key = eval(key)
+        key = json.loads(key)
         return key
 
 
     def get_link(self, thing_id: str) -> tuple:
         req = self.client.get(f"{self.base_url}/ajax/sources/{thing_id}").json()["link"]
         print(req)
         return req, self.rabbit_id(req)
```

### Comparing `mov_cli-1.5.0/mov_cli/websites/indian/einthusan.py` & `mov_cli-1.5.1/mov_cli/websites/indian/einthusan.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/websites/indian/streamblasters.py` & `mov_cli-1.5.1/mov_cli/websites/indian/streamblasters.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/websites/indian/tamilyogi.py` & `mov_cli-1.5.1/mov_cli/websites/indian/tamilyogi.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/websites/international/wlext.py` & `mov_cli-1.5.1/mov_cli/websites/international/wlext.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/websites/livetv/eja.py` & `mov_cli-1.5.1/mov_cli/websites/livetv/eja.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/websites/sports/scdn.py` & `mov_cli-1.5.1/mov_cli/websites/sports/scdn.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/websites/turkish/turkish123.py` & `mov_cli-1.5.1/mov_cli/websites/turkish/turkish123.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/mov_cli/websites/turkish/yoturkish.py` & `mov_cli-1.5.1/mov_cli/websites/turkish/yoturkish.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.5.0/pyproject.toml` & `mov_cli-1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mov-cli"
-version = "1.5.0"
+version = "1.5.1"
 description = "A cli tool to browse and watch Movies/Shows/TV/Sports."
 authors = ["Pain <painedposeidon444@gmail.com>"]
 maintainers = ["Ananas <ananas@r3tr0ananas.lol>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "mov_cli"}]
 repository = "https://github.com/mov-cli/mov-cli"
@@ -22,8 +22,8 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 mov-cli = "mov_cli.__main__:movcli"
 
 [tool.poetry.urls]
-"Bug Tracker" = "https://github.com/mov-cli/mov-cli/issues"
+"Bug Tracker" = "https://github.com/mov-cli/mov-cli/issues"
```

### Comparing `mov_cli-1.5.0/PKG-INFO` & `mov_cli-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 1.5.0
+Version: 1.5.1
 Summary: A cli tool to browse and watch Movies/Shows/TV/Sports.
 Home-page: https://github.com/mov-cli/mov-cli
 License: GPLv3
 Author: Pain
 Author-email: painedposeidon444@gmail.com
 Maintainer: Ananas
 Maintainer-email: ananas@r3tr0ananas.lol
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 1.5.0 Summary: A cli tool to
+Metadata-Version: 2.1 Name: mov-cli Version: 1.5.1 Summary: A cli tool to
 browse and watch Movies/Shows/TV/Sports. Home-page: https://github.com/mov-cli/
 mov-cli License: GPLv3 Author: Pain Author-email: painedposeidon444@gmail.com
 Maintainer: Ananas Maintainer-email: ananas@r3tr0ananas.lol Requires-Python:
 >=3.9,<4.0 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: beautifulsoup4
```

