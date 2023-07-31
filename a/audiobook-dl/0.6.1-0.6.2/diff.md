# Comparing `tmp/audiobook-dl-0.6.1.tar.gz` & `tmp/audiobook-dl-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiobook-dl-0.6.1.tar", last modified: Mon Jul 10 20:02:46 2023, max compression
+gzip compressed data, was "audiobook-dl-0.6.2.tar", last modified: Mon Jul 31 08:06:55 2023, max compression
```

## Comparing `audiobook-dl-0.6.1.tar` & `audiobook-dl-0.6.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.514252 audiobook-dl-0.6.1/
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.490252 audiobook-dl-0.6.1/.github/
--rw-r--r--   0 jo1gi     (1000) users      (100)       13 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/.github/FUNDING.yml
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.490252 audiobook-dl-0.6.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 jo1gi     (1000) users      (100)      349 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/.github/ISSUE_TEMPLATE/bug_report.md
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.491252 audiobook-dl-0.6.1/.github/workflows/
--rw-r--r--   0 jo1gi     (1000) users      (100)      315 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/.github/workflows/ci.yml
--rw-r--r--   0 jo1gi     (1000) users      (100)      310 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/.github/workflows/pytest.yml
--rw-r--r--   0 jo1gi     (1000) users      (100)      539 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/.gitignore
--rw-r--r--   0 jo1gi     (1000) users      (100)    35149 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/LICENSE
--rw-r--r--   0 jo1gi     (1000) users      (100)     5369 2023-07-10 20:02:46.514252 audiobook-dl-0.6.1/PKG-INFO
--rw-r--r--   0 jo1gi     (1000) users      (100)     4798 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/README.md
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.493252 audiobook-dl-0.6.1/audiobook_dl.egg-info/
--rw-r--r--   0 jo1gi     (1000) users      (100)     5369 2023-07-10 20:02:46.000000 audiobook-dl-0.6.1/audiobook_dl.egg-info/PKG-INFO
--rw-r--r--   0 jo1gi     (1000) users      (100)     2311 2023-07-10 20:02:46.000000 audiobook-dl-0.6.1/audiobook_dl.egg-info/SOURCES.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)        1 2023-07-10 20:02:46.000000 audiobook-dl-0.6.1/audiobook_dl.egg-info/dependency_links.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       59 2023-07-10 20:02:46.000000 audiobook-dl-0.6.1/audiobook_dl.egg-info/entry_points.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       88 2023-07-10 20:02:46.000000 audiobook-dl-0.6.1/audiobook_dl.egg-info/requires.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       12 2023-07-10 20:02:46.000000 audiobook-dl-0.6.1/audiobook_dl.egg-info/top_level.txt
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.495252 audiobook-dl-0.6.1/audiobookdl/
--rw-r--r--   0 jo1gi     (1000) users      (100)      191 2023-07-10 19:59:26.000000 audiobook-dl-0.6.1/audiobookdl/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     5968 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/__main__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     3495 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/args.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.496252 audiobook-dl-0.6.1/audiobookdl/assets/
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.500252 audiobook-dl-0.6.1/audiobookdl/assets/errors/
--rw-r--r--   0 jo1gi     (1000) users      (100)      221 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/errors/book_access.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      179 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/errors/chapters_add.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       56 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/errors/config_not_found.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      468 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/errors/data_not_present.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       45 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/errors/failed_combining.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       66 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/errors/missing_dependency.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      179 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/errors/no_files_found.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      107 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/errors/no_source_found.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       55 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/errors/request_error.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      273 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/errors/user_not_authorized.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)       65 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/ffmpeg_chapter_template.txt
--rw-r--r--   0 jo1gi     (1000) users      (100)      317 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/assets/simple_help.txt
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.486252 audiobook-dl-0.6.1/audiobookdl/assets/sources/
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.503252 audiobook-dl-0.6.1/audiobookdl/assets/sources/podimo/
--rw-r--r--   0 jo1gi     (1000) users      (100)     1010 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/assets/sources/podimo/book_info.graphql
--rw-r--r--   0 jo1gi     (1000) users      (100)      108 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/assets/sources/podimo/files.graphql
--rw-r--r--   0 jo1gi     (1000) users      (100)      270 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/assets/sources/podimo/login.graphql
--rw-r--r--   0 jo1gi     (1000) users      (100)     1488 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/assets/sources/podimo/podcast.graphql
--rw-r--r--   0 jo1gi     (1000) users      (100)      185 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/assets/sources/podimo/podcast_episode_file.graphql
--rw-r--r--   0 jo1gi     (1000) users      (100)      866 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/assets/sources/podimo/podcast_episodes.graphql
--rw-r--r--   0 jo1gi     (1000) users      (100)     1983 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/config.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1342 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/exceptions.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1407 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/logging.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.505252 audiobook-dl-0.6.1/audiobookdl/output/
--rw-r--r--   0 jo1gi     (1000) users      (100)       40 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/output/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     8073 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/output/download.py
--rw-r--r--   0 jo1gi     (1000) users      (100)      641 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/output/encryption.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.506252 audiobook-dl-0.6.1/audiobookdl/output/metadata/
--rw-r--r--   0 jo1gi     (1000) users      (100)     1363 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/output/metadata/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1524 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/output/metadata/ffmpeg.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     2391 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/output/metadata/id3.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1476 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/output/metadata/mp4.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     3473 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/output/output.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.511252 audiobook-dl-0.6.1/audiobookdl/sources/
--rw-r--r--   0 jo1gi     (1000) users      (100)     1637 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     2050 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/audiobooksdotcom.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     4654 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/bookbeat.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     4318 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/chirp.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     3510 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/ereolen.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1325 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/librivox.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     5289 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/nextory.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     3308 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/overdrive.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     7927 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/podimo.py
--rw-r--r--   0 jo1gi     (1000) users      (100)      155 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/sources/rss.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     4413 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/saxo.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     6258 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/scribd.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.512252 audiobook-dl-0.6.1/audiobookdl/sources/source/
--rw-r--r--   0 jo1gi     (1000) users      (100)     5125 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/source/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     2404 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/audiobookdl/sources/source/networking.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     5819 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/storytel.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     4717 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/sources/yourcloudlibrary.py
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.512252 audiobook-dl-0.6.1/audiobookdl/utils/
--rw-r--r--   0 jo1gi     (1000) users      (100)     1159 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/utils/__init__.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     4028 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/audiobookdl/utils/audiobook.py
--rw-r--r--   0 jo1gi     (1000) users      (100)     1318 2023-07-10 19:58:47.000000 audiobook-dl-0.6.1/pyproject.toml
--rw-r--r--   0 jo1gi     (1000) users      (100)       38 2023-07-10 20:02:46.514252 audiobook-dl-0.6.1/setup.cfg
--rw-r--r--   0 jo1gi     (1000) users      (100)       38 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/setup.py
--rw-r--r--   0 jo1gi     (1000) users      (100)      434 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/shell.nix
--rw-r--r--   0 jo1gi     (1000) users      (100)     2139 2023-07-06 17:09:06.000000 audiobook-dl-0.6.1/supported_sites.md
-drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-10 20:02:46.513252 audiobook-dl-0.6.1/tests/
--rw-r--r--   0 jo1gi     (1000) users      (100)     1087 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/tests/test_output.py
--rw-r--r--   0 jo1gi     (1000) users      (100)      970 2023-07-01 12:46:04.000000 audiobook-dl-0.6.1/tests/test_urls.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-31 08:06:55.775601 audiobook-dl-0.6.2/
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-31 08:06:55.762601 audiobook-dl-0.6.2/.github/
+-rw-r--r--   0 jo1gi     (1000) users      (100)       13 2023-04-16 16:16:37.000000 audiobook-dl-0.6.2/.github/FUNDING.yml
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-31 08:06:55.762601 audiobook-dl-0.6.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 jo1gi     (1000) users      (100)      349 2023-04-16 16:16:37.000000 audiobook-dl-0.6.2/.github/ISSUE_TEMPLATE/bug_report.md
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-31 08:06:55.762601 audiobook-dl-0.6.2/.github/workflows/
+-rw-r--r--   0 jo1gi     (1000) users      (100)      315 2023-04-16 16:16:37.000000 audiobook-dl-0.6.2/.github/workflows/ci.yml
+-rw-r--r--   0 jo1gi     (1000) users      (100)      310 2023-04-16 16:16:37.000000 audiobook-dl-0.6.2/.github/workflows/pytest.yml
+-rw-r--r--   0 jo1gi     (1000) users      (100)      539 2023-04-16 16:16:37.000000 audiobook-dl-0.6.2/.gitignore
+-rw-r--r--   0 jo1gi     (1000) users      (100)    35149 2023-04-16 16:16:37.000000 audiobook-dl-0.6.2/LICENSE
+-rw-r--r--   0 jo1gi     (1000) users      (100)     5369 2023-07-31 08:06:55.775601 audiobook-dl-0.6.2/PKG-INFO
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4798 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/README.md
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-31 08:06:55.762601 audiobook-dl-0.6.2/audiobook_dl.egg-info/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     5369 2023-07-31 08:06:55.000000 audiobook-dl-0.6.2/audiobook_dl.egg-info/PKG-INFO
+-rw-r--r--   0 jo1gi     (1000) users      (100)     2311 2023-07-31 08:06:55.000000 audiobook-dl-0.6.2/audiobook_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)        1 2023-07-31 08:06:55.000000 audiobook-dl-0.6.2/audiobook_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       59 2023-07-31 08:06:55.000000 audiobook-dl-0.6.2/audiobook_dl.egg-info/entry_points.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       94 2023-07-31 08:06:55.000000 audiobook-dl-0.6.2/audiobook_dl.egg-info/requires.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       12 2023-07-31 08:06:55.000000 audiobook-dl-0.6.2/audiobook_dl.egg-info/top_level.txt
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-31 08:06:55.763601 audiobook-dl-0.6.2/audiobookdl/
+-rw-r--r--   0 jo1gi     (1000) users      (100)      191 2023-07-31 08:04:01.000000 audiobook-dl-0.6.2/audiobookdl/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     5968 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/__main__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     3495 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/args.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-31 08:06:55.763601 audiobook-dl-0.6.2/audiobookdl/assets/
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-31 08:06:55.772601 audiobook-dl-0.6.2/audiobookdl/assets/errors/
+-rw-r--r--   0 jo1gi     (1000) users      (100)      221 2023-04-16 16:16:37.000000 audiobook-dl-0.6.2/audiobookdl/assets/errors/book_access.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      179 2023-04-16 16:16:37.000000 audiobook-dl-0.6.2/audiobookdl/assets/errors/chapters_add.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       56 2023-05-07 20:52:41.000000 audiobook-dl-0.6.2/audiobookdl/assets/errors/config_not_found.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      468 2023-04-16 16:16:37.000000 audiobook-dl-0.6.2/audiobookdl/assets/errors/data_not_present.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       45 2023-04-16 16:16:37.000000 audiobook-dl-0.6.2/audiobookdl/assets/errors/failed_combining.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       66 2023-04-16 16:16:37.000000 audiobook-dl-0.6.2/audiobookdl/assets/errors/missing_dependency.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      179 2023-04-16 16:16:37.000000 audiobook-dl-0.6.2/audiobookdl/assets/errors/no_files_found.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      107 2023-04-16 16:16:37.000000 audiobook-dl-0.6.2/audiobookdl/assets/errors/no_source_found.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       55 2023-04-16 16:16:37.000000 audiobook-dl-0.6.2/audiobookdl/assets/errors/request_error.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      273 2023-04-16 16:16:37.000000 audiobook-dl-0.6.2/audiobookdl/assets/errors/user_not_authorized.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)       65 2023-04-16 16:16:37.000000 audiobook-dl-0.6.2/audiobookdl/assets/ffmpeg_chapter_template.txt
+-rw-r--r--   0 jo1gi     (1000) users      (100)      317 2023-04-16 16:16:37.000000 audiobook-dl-0.6.2/audiobookdl/assets/simple_help.txt
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-31 08:06:55.753601 audiobook-dl-0.6.2/audiobookdl/assets/sources/
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-31 08:06:55.773601 audiobook-dl-0.6.2/audiobookdl/assets/sources/podimo/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1010 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/assets/sources/podimo/book_info.graphql
+-rw-r--r--   0 jo1gi     (1000) users      (100)      108 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/assets/sources/podimo/files.graphql
+-rw-r--r--   0 jo1gi     (1000) users      (100)      270 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/assets/sources/podimo/login.graphql
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1488 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/assets/sources/podimo/podcast.graphql
+-rw-r--r--   0 jo1gi     (1000) users      (100)      185 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/assets/sources/podimo/podcast_episode_file.graphql
+-rw-r--r--   0 jo1gi     (1000) users      (100)      866 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/assets/sources/podimo/podcast_episodes.graphql
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1983 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/config.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1342 2023-05-07 20:52:12.000000 audiobook-dl-0.6.2/audiobookdl/exceptions.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1407 2023-06-20 10:50:30.000000 audiobook-dl-0.6.2/audiobookdl/logging.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-31 08:06:55.773601 audiobook-dl-0.6.2/audiobookdl/output/
+-rw-r--r--   0 jo1gi     (1000) users      (100)       40 2023-04-16 16:16:37.000000 audiobook-dl-0.6.2/audiobookdl/output/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     8073 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/output/download.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)      641 2023-04-16 16:16:37.000000 audiobook-dl-0.6.2/audiobookdl/output/encryption.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-31 08:06:55.774601 audiobook-dl-0.6.2/audiobookdl/output/metadata/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1363 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/output/metadata/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1524 2023-06-20 11:00:09.000000 audiobook-dl-0.6.2/audiobookdl/output/metadata/ffmpeg.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     2391 2023-06-20 10:59:51.000000 audiobook-dl-0.6.2/audiobookdl/output/metadata/id3.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1476 2023-04-16 16:16:37.000000 audiobook-dl-0.6.2/audiobookdl/output/metadata/mp4.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     3473 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/output/output.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-31 08:06:55.775601 audiobook-dl-0.6.2/audiobookdl/sources/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1637 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/sources/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     2521 2023-07-29 16:36:36.000000 audiobook-dl-0.6.2/audiobookdl/sources/audiobooksdotcom.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4654 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/sources/bookbeat.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4318 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/sources/chirp.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     3510 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/sources/ereolen.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1325 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/sources/librivox.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     5289 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/sources/nextory.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     3308 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/sources/overdrive.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     7899 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/sources/podimo.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)      155 2023-04-16 16:16:37.000000 audiobook-dl-0.6.2/audiobookdl/sources/rss.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4413 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/sources/saxo.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     6258 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/sources/scribd.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-31 08:06:55.775601 audiobook-dl-0.6.2/audiobookdl/sources/source/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     5219 2023-07-29 16:36:36.000000 audiobook-dl-0.6.2/audiobookdl/sources/source/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     2404 2023-06-20 10:51:00.000000 audiobook-dl-0.6.2/audiobookdl/sources/source/networking.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     5878 2023-07-26 16:22:08.000000 audiobook-dl-0.6.2/audiobookdl/sources/storytel.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4403 2023-07-28 20:55:16.000000 audiobook-dl-0.6.2/audiobookdl/sources/yourcloudlibrary.py
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-31 08:06:55.775601 audiobook-dl-0.6.2/audiobookdl/utils/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1159 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/utils/__init__.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     4028 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/audiobookdl/utils/audiobook.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1332 2023-07-26 16:23:05.000000 audiobook-dl-0.6.2/pyproject.toml
+-rw-r--r--   0 jo1gi     (1000) users      (100)       38 2023-07-31 08:06:55.775601 audiobook-dl-0.6.2/setup.cfg
+-rw-r--r--   0 jo1gi     (1000) users      (100)       38 2023-04-16 16:16:37.000000 audiobook-dl-0.6.2/setup.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)      434 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/shell.nix
+-rw-r--r--   0 jo1gi     (1000) users      (100)     2139 2023-07-26 13:02:13.000000 audiobook-dl-0.6.2/supported_sites.md
+drwxr-xr-x   0 jo1gi     (1000) users      (100)        0 2023-07-31 08:06:55.775601 audiobook-dl-0.6.2/tests/
+-rw-r--r--   0 jo1gi     (1000) users      (100)     1087 2023-04-19 19:52:07.000000 audiobook-dl-0.6.2/tests/test_output.py
+-rw-r--r--   0 jo1gi     (1000) users      (100)      970 2023-04-16 16:16:37.000000 audiobook-dl-0.6.2/tests/test_urls.py
```

### Comparing `audiobook-dl-0.6.1/.gitignore` & `audiobook-dl-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/LICENSE` & `audiobook-dl-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/PKG-INFO` & `audiobook-dl-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiobook-dl
-Version: 0.6.1
+Version: 0.6.2
 Summary: CLI tool for downloading audiobooks from online sources
 Author-email: Joakim Holm <mail@joakimholm.xyz>
 Project-URL: Homepage, https://github.com/jo1gi/audiobook-dl
 Project-URL: Bugtracker, https://github.com/jo1gi/audiobook-dl/issues
 Keywords: audiobooks,cli,downloader
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `audiobook-dl-0.6.1/README.md` & `audiobook-dl-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobook_dl.egg-info/PKG-INFO` & `audiobook-dl-0.6.2/audiobook_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiobook-dl
-Version: 0.6.1
+Version: 0.6.2
 Summary: CLI tool for downloading audiobooks from online sources
 Author-email: Joakim Holm <mail@joakimholm.xyz>
 Project-URL: Homepage, https://github.com/jo1gi/audiobook-dl
 Project-URL: Bugtracker, https://github.com/jo1gi/audiobook-dl/issues
 Keywords: audiobooks,cli,downloader
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `audiobook-dl-0.6.1/audiobook_dl.egg-info/SOURCES.txt` & `audiobook-dl-0.6.2/audiobook_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/__main__.py` & `audiobook-dl-0.6.2/audiobookdl/__main__.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/args.py` & `audiobook-dl-0.6.2/audiobookdl/args.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/assets/sources/podimo/book_info.graphql` & `audiobook-dl-0.6.2/audiobookdl/assets/sources/podimo/book_info.graphql`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/assets/sources/podimo/podcast.graphql` & `audiobook-dl-0.6.2/audiobookdl/assets/sources/podimo/podcast.graphql`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/assets/sources/podimo/podcast_episodes.graphql` & `audiobook-dl-0.6.2/audiobookdl/assets/sources/podimo/podcast_episodes.graphql`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/config.py` & `audiobook-dl-0.6.2/audiobookdl/config.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/exceptions.py` & `audiobook-dl-0.6.2/audiobookdl/exceptions.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/logging.py` & `audiobook-dl-0.6.2/audiobookdl/logging.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/output/download.py` & `audiobook-dl-0.6.2/audiobookdl/output/download.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/output/encryption.py` & `audiobook-dl-0.6.2/audiobookdl/output/encryption.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/output/metadata/__init__.py` & `audiobook-dl-0.6.2/audiobookdl/output/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/output/metadata/ffmpeg.py` & `audiobook-dl-0.6.2/audiobookdl/output/metadata/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/output/metadata/id3.py` & `audiobook-dl-0.6.2/audiobookdl/output/metadata/id3.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/output/metadata/mp4.py` & `audiobook-dl-0.6.2/audiobookdl/output/metadata/mp4.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/output/output.py` & `audiobook-dl-0.6.2/audiobookdl/output/output.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/sources/__init__.py` & `audiobook-dl-0.6.2/audiobookdl/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/sources/audiobooksdotcom.py` & `audiobook-dl-0.6.2/audiobookdl/sources/audiobooksdotcom.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 from .source import Source
 from audiobookdl import AudiobookFile, logging, AudiobookMetadata, Cover, Audiobook
-from audiobookdl.exceptions import NoSourceFound
+from audiobookdl.exceptions import NoSourceFound, DataNotPresent
 
 import re
 from typing import List
 from urllib.parse import unquote
 from urllib3.util import parse_url
+import requests
 
 BASEURL = "https://www.audiobooks.com/book/stream/"
 
 
 class AudiobooksdotcomSource(Source):
     match = [
         r"{}\d+(/\d)?".format(BASEURL)
     ]
     names = [ "audiobooks.com" ]
 
     def download(self, url: str) -> Audiobook:
         path = parse_url(url).path
         if not path:
             raise NoSourceFound
+        # User-Agent has to match the one in the cookies
+        user_agent = self.extract_useragent_from_cookies()
+        logging.debug(f"{user_agent=}")
+        self._session.headers.update({"User-Agent": user_agent})
         book_id = path.split("/")[3]
         scrape_url = f"{BASEURL}{book_id}/1"
         return Audiobook(
             session = self._session,
-            metadata = self.get_metadata(scrape_url),
-            cover = self.get_cover(scrape_url),
-            files = self.get_files(scrape_url),
+            metadata = self.extract_metadata(scrape_url),
+            cover = self.download_cover(scrape_url),
+            files = self.extract_file(scrape_url),
         )
 
 
-    def get_metadata(self, scrape_url: str) -> AudiobookMetadata:
+    def extract_metadata(self, scrape_url: str) -> AudiobookMetadata:
         title = self.find_elem_in_page(scrape_url, "h2#bookTitle")
         return AudiobookMetadata(title)
 
 
-    def get_cover(self, scrape_url: str) -> Cover:
+    def download_cover(self, scrape_url: str) -> Cover:
         cover_url = "http:" + \
             self.find_elem_in_page(
                 scrape_url,
                 "img.bookimage",
                 data="src"
             )
         return Cover(self.get(cover_url), "jpg")
@@ -51,17 +56,25 @@
 
         :returns: User-Agent string
         """
         raw = self._session.cookies.get("ci_session", domain="www.audiobooks.com")
         return unquote(raw).split("\"")[11]
 
 
-    def get_files(self, scrape_url: str) -> List[AudiobookFile]:
-        media_url = self.find_in_page(
+    def extract_file(self, scrape_url: str) -> List[AudiobookFile]:
+        """
+        Extract audio url from html page
+
+        :param scrape_url: Url of page to scrape for audio link
+        :returns: List of audio files with a single file in it
+        """
+        response = self._session.get(
             scrape_url,
-            r"(?<=(mp3: \")).+(?=(&rs))",
-            headers = {
-                # User agent has to match the one in the cookies
-                "User-Agent": self.extract_useragent_from_cookies()
-            }
         )
-        return [ AudiobookFile(url=media_url, ext="mp3") ]
+        audio_match = re.search(
+            r'(?<=(mp3: ")).+(?=(&rs))',
+            response.text
+        )
+        if audio_match is None:
+            raise DataNotPresent
+        audio_url = audio_match.group()
+        return [ AudiobookFile(url=audio_url, ext="mp3") ]
```

### Comparing `audiobook-dl-0.6.1/audiobookdl/sources/bookbeat.py` & `audiobook-dl-0.6.2/audiobookdl/sources/bookbeat.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/sources/chirp.py` & `audiobook-dl-0.6.2/audiobookdl/sources/chirp.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/sources/ereolen.py` & `audiobook-dl-0.6.2/audiobookdl/sources/ereolen.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/sources/librivox.py` & `audiobook-dl-0.6.2/audiobookdl/sources/librivox.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/sources/nextory.py` & `audiobook-dl-0.6.2/audiobookdl/sources/nextory.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/sources/overdrive.py` & `audiobook-dl-0.6.2/audiobookdl/sources/overdrive.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/sources/podimo.py` & `audiobook-dl-0.6.2/audiobookdl/sources/podimo.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 
     def download_podcast_metadata(self, podcast_id: str) -> dict:
         response = self.graphql_request(
             operation_name = "PodcastResultsQuery",
             query = "podcast",
             variables = {
-                "id": "2e798fcd-09f8-42d5-af21-3cc9babcb5d2"
+                "id": podcast_id
             }
         )
         return response.json()["data"]["podcastById"]
 
 
     def download_podcast_episode_ids(self, podcast_id: str) -> List:
         response = self.graphql_request(
```

### Comparing `audiobook-dl-0.6.1/audiobookdl/sources/saxo.py` & `audiobook-dl-0.6.2/audiobookdl/sources/saxo.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/sources/scribd.py` & `audiobook-dl-0.6.2/audiobookdl/sources/scribd.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/sources/source/__init__.py` & `audiobook-dl-0.6.2/audiobookdl/sources/source/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,19 +93,20 @@
 
 
     def download(self, url: str) -> Result:
         """Download book or series"""
         raise NotImplementedError
 
 
-    def _get_page(self, url: str, **kwargs) -> bytes:
+    def _get_page(self, url: str, use_cache: bool = True, **kwargs) -> bytes:
         """Download a page and caches it"""
-        if url not in self.__pages:
+        if url not in self.__pages and use_cache:
             resp = self.get(url, **kwargs)
-            self.__pages[url] = resp
+            if use_cache:
+                self.__pages[url] = resp
         return self.__pages[url]
 
 
     def find_elem_in_page(self, url: str, selector: str, data=None, **kwargs):
         """
         Find the first html element in page from `url` that matches `selector`.
         Will return the attribute specified in `data`. Will return element text
@@ -136,14 +137,15 @@
 
     def find_in_page(self, url: str, regex: str, group_index: int = 0, **kwargs) -> str:
         """
         Find some text in a page based on a regex.
         Will cache the page.
         """
         page = self._get_page(url, **kwargs).decode("utf8")
+        print(f"{page=}")
         m = re.search(regex, page)
         if m is None:
             logging.debug(f"Could not find match from {url} with {regex}")
             raise DataNotPresent
         return m.group(group_index)
```

### Comparing `audiobook-dl-0.6.1/audiobookdl/sources/source/networking.py` & `audiobook-dl-0.6.2/audiobookdl/sources/source/networking.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/sources/storytel.py` & `audiobook-dl-0.6.2/audiobookdl/sources/storytel.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                 "pwd": password,
             }
         )
         if resp.status_code != 200:
             raise UserNotAuthorized
         user_data = resp.json()
         jwt = user_data["accountInfo"]["jwt"]
-        self.single_signon_token = user_data["singleSignToken"]
+        self.single_signon_token = user_data["accountInfo"]["singleSignToken"]
         self._session.headers.update({"authorization": f"Bearer {jwt}"})
 
 
     def download(self, url: str) -> Audiobook:
         book_id = url.split("-")[-1]
         bookshelf = self.download_bookshelf()
         book_info = self.find_book_info(bookshelf, book_id)
@@ -84,14 +84,15 @@
         """
         Find book matching book_id in user bookshelf
 
         :param bookshelf: Users current listening boooks
         :param book_id: Id of book to download
         :returns: Book information
         """
+        bookshelf = bookshelf.json()
         for book in bookshelf["books"]:
             if book["book"]["consumableId"] == book_id:
                 return book
         raise MissingBookAccess
 
 
 
@@ -131,18 +132,18 @@
     def download_audiobook_info(self, book_info):
         """Download information about the audiobook files"""
         consumable_id = book_info["book"]["consumableId"]
         url = f"https://api.storytel.net/playback-metadata/consumable/{consumable_id}"
         file_metadata = self._session.get(url).json()
         if not "formats" in file_metadata:
             raise DataNotPresent
-        for format in storytel_metadata["formats"]:
+        for format in file_metadata["formats"]:
             if format["type"] == "abook":
                 return format
-        raise DataNotPresnt
+        raise DataNotPresent
 
 
     @staticmethod
     def create_chapter(start_time: int, chapter_info) -> Chapter:
         """Create chapter object"""
         if "title" in chapter_info:
             title = chapter_info["title"]
@@ -160,11 +161,11 @@
         for chapter in file_metadata["chapters"]:
             chapters.append(self.create_chapter(start_time, chapter))
             start_time += chapter["durationInMilliseconds"]
         return chapters
 
 
     def download_cover(self, book_info) -> Cover:
-        isbn = book_info["isbn"]
+        isbn = book_info["abook"]["iisbn"]
         cover_url = f"https://www.storytel.com/images/{isbn}/640x640/cover.jpg"
         cover_data = self.get(cover_url)
         return Cover(cover_data, "jpg")
```

### Comparing `audiobook-dl-0.6.1/audiobookdl/sources/yourcloudlibrary.py` & `audiobook-dl-0.6.2/audiobookdl/sources/yourcloudlibrary.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,147 +1,134 @@
 from .source import Source
-from audiobookdl import AudiobookFile, logging, AudiobookMetadata, Cover, Audiobook
+from audiobookdl import AudiobookFile, logging, AudiobookMetadata, Cover, Audiobook, Chapter
 from audiobookdl.exceptions import UserNotAuthorized, RequestError
 
 import requests.utils
 import base64
 from typing import List
 
 class YourCloudLibrarySource(Source):
     match = [
-        r"https?://ebook.yourcloudlibrary.com/library/[^/]+/AudioPlayer/.+"
+        # r"https?://ebook.yourcloudlibrary.com/library/[^/]+/AudioPlayer/.+"
+        r"https?://audio.yourcloudlibrary.com/listen/.+"
     ]
     names = [ "YourCloudLibrary" ]
+    login_data = [ "username", "password", "library" ]
     _authentication_methods = [
         "cookies",
         "login"
     ]
+    _library: str
 
     def download(self, url: str) -> Audiobook:
-        fullfillment_token = self.download_fullfillment_token(url)
-        book_info = self.download_book_info(url)
-        library = self.extract_library_id(url)
-        audioplayer = self.post_json(
-            f"https://ebook.yourcloudlibrary.com/uisvc/{library}/AudioPlayer",
-            data = {
-                "url": f"{book_info['fullfillmentTokenUrl']}&token={fullfillment_token}"
-            }
-        )
-        fulfillment_id = audioplayer["fulfillmentId"]
-        account_id = audioplayer["accountId"]
-        session_key = audioplayer["sessionKey"]
-        headers = { "Session-Key": session_key }
-        meta = self.get_json(
-            f"https://api.findawayworld.com/v4/accounts/{account_id}/audiobooks/{fulfillment_id}",
-            headers=headers
-        )
-        playlist = self.post_json(
-            f"https://api.findawayworld.com/v4/audiobooks/{fulfillment_id}/playlists",
-            json = {
-                "license_id": audioplayer["licenseId"]
-            },
-            headers=headers
-        )
+        account_id = self.extract_json_string(url, "accountId")
+        logging.debug(f"{account_id=}")
+        fulfillment_id = self.extract_json_string(url, "fulfillmentId")
+        logging.debug(f"{fulfillment_id=}")
+        license_id = self.extract_json_string(url, "licenseId")
+        logging.debug(f"{license_id=}")
+        session_key = self.extract_json_string(url, "session_key")
+        self._session.headers.update({"Session-Key": session_key})
+        book_info = self.download_book_info(account_id, fulfillment_id)
+        playlist = self.download_playlist(fulfillment_id, license_id)
         return Audiobook(
             session = self._session,
             files = self.get_files(playlist),
-            metadata = self.get_metadata(book_info, meta),
-            cover = self.download_cover(meta),
+            metadata = self.get_metadata(book_info),
+            cover = self.download_cover(book_info),
+            chapters = self.create_chapters(book_info)
+        )
+
+
+    def extract_json_string(self, url: str, key: str) -> str:
+        """
+        Extracts string from json in web page
+
+        :param url: Url of page to extract from
+        :param key: Key of value to extract
+        :returns: Value
+        """
+        return self.find_in_page(
+            url,
+            fr"(?<=(\"{key}\":\"))[^\"]+",
+            force_cookies = True,
         )
 
 
     @staticmethod
-    def get_files(playlist) -> List[AudiobookFile]:
+    def get_files(playlist: dict) -> List[AudiobookFile]:
         files = []
         for f in playlist["playlist"]:
             files.append(AudiobookFile(
                 url = f["url"],
                 ext = "mp3"
             ))
         return files
 
 
-    def get_metadata(self, book_info, meta) -> AudiobookMetadata:
-        title = book_info["Title"]
-        metadata = AudiobookMetadata(title)
-        if not meta is None:
-            audiobook = meta["audiobook"]
-            metadata.add_authors(audiobook["authors"])
-            metadata.add_narrators(audiobook["narrators"])
-            if audiobook["series"] is not None and len(audiobook["series"]) >= 1:
-                metadata.series = audiobook["series"][0]
+    @staticmethod
+    def get_metadata(book_info: dict) -> AudiobookMetadata:
+        metadata = AudiobookMetadata(
+            title = book_info["title"],
+            authors = book_info["authors"],
+            narrators = book_info["narrators"]
+        )
+        if book_info["series"] is not None and len(book_info["series"]) >= 1:
+            metadata.series = book_info["series"][0]
         return metadata
 
 
     def download_cover(self, meta) -> Cover:
-        cover_url = meta['audiobook']['cover_url']
-        cover_data = self.get(cover_url)
+        cover_url = meta['cover_url']
+        cover_data = self.get(f"{cover_url}?aspect=1:1")
         return Cover(cover_data, "jpg")
 
 
     @staticmethod
-    def extract_library_id(url: str) -> str:
-        """
-        Extract library id from url
+    def create_chapters(book_info: dict) -> List[Chapter]:
+        chapters = []
+        time = 0
+        for chapter in book_info["chapters"]:
+            time += chapter["duration"]
+            chapters.append(
+                Chapter(
+                    start = time,
+                    title = f"Chapter {chapter['chapter_number']}"
+                )
+            )
+        return chapters
 
-        :param url: Url 
-        :returns: Library id
+    def download_book_info(self, account_id: str, fulfillment_id: str) -> dict:
         """
-        return url.split("/")[-3]
-
-
-    def download_fullfillment_token(self, url: str) -> str:
-        """
-        Download and extract fullfillment token
+        Download metadata about book
 
         :param url: Book url
-        :returns: Fullfillment token
+        :param fulfillment_id: Id used for book
+        :returns: Metadata about book
         """
-        token_base64 = self.find_in_page(
-            url,
-            r"(?<=(\"Osi\":\"x-))[^\"]+",
-            force_cookies = True,
-        )
-        if token_base64 is None:
-            raise UserNotAuthorized
-        token = base64.b64decode(token_base64).decode('utf8')
-        logging.debug(f"{token=}")
-        return token
+        return self.get_json(
+            f"https://api.findawayworld.com/v4/accounts/{account_id}/audiobooks/{fulfillment_id}",
+            force_cookies = True
+        )["audiobook"]
 
 
-    def download_book_info(self, url: str) -> dict:
+    def download_playlist(self, fulfillment_id: str, license_id: str) -> dict:
         """
-        Download metadata about book
-
-        :param url: Book url
-        :returns: Metadata about book
+        Download list of audio files
         """
-        # Get list of borrowed books
-        library = self.extract_library_id(url)
-        borrowed = self.get_json(
-            f"https://ebook.yourcloudlibrary.com/uisvc/{library}/Patron/Borrowed",
-            force_cookies = True
+        license_str = f'{{"license_id":"{license_id}"}}'
+        return self.post_json(
+            f"https://api.findawayworld.com/v4/audiobooks/{fulfillment_id}/playlists",
+            data = license_str
         )
-        if borrowed is None:
-            raise UserNotAuthorized
-        # Find the matching book in list of borrowed books
-        url_id = url.split("/")[-1]
-        book_info = None
-        for i in borrowed:
-            if i["Id"] == url_id:
-                book_info = i
-        if book_info is None:
-            raise UserNotAuthorized
-        return book_info
 
 
-    def _login(self, url: str, username: str, password: str):
-        library = self.extract_library_id(url)
+    def _login(self, url: str, username: str, password: str, library: str): # type: ignore
+        self.library = library
         resp = self.post(
-            f"https://ebook.yourcloudlibrary.com/uisvc/{library}/Patron/LoginPatron",
+            f"https://ebook.yourcloudlibrary.com/library/{library}/?_data=root",
             data = {
-                "UserId": username,
-                "Password": password
+                "action": "login",
+                "barcode": username,
+                "pin": password
             }
         )
-        # TODO Validate authentication
-        logging.debug(f"Authentication response {resp.decode('utf8')}")
```

### Comparing `audiobook-dl-0.6.1/audiobookdl/utils/__init__.py` & `audiobook-dl-0.6.2/audiobookdl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/audiobookdl/utils/audiobook.py` & `audiobook-dl-0.6.2/audiobookdl/utils/audiobook.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/pyproject.toml` & `audiobook-dl-0.6.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -12,24 +12,25 @@
 keywords = ["audiobooks", "cli", "downloader"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Topic :: Multimedia :: Sound/Audio",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 ]
 dependencies = [
-    "requests",
+    "attrs",
+    "cssselect",
+    "importlib-resources",
     "lxml",
-    "rich",
+    "m3u8",
     "mutagen",
     "pillow",
-    "cssselect",
-    "m3u8",
     "pycryptodome",
-    "importlib-resources",
-    "attrs"
+    "requests",
+    "rich",
+    "tomli",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/jo1gi/audiobook-dl"
 "Bugtracker" = "https://github.com/jo1gi/audiobook-dl/issues"
```

### Comparing `audiobook-dl-0.6.1/supported_sites.md` & `audiobook-dl-0.6.2/supported_sites.md`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/tests/test_output.py` & `audiobook-dl-0.6.2/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `audiobook-dl-0.6.1/tests/test_urls.py` & `audiobook-dl-0.6.2/tests/test_urls.py`

 * *Files identical despite different names*

