# Comparing `tmp/sentiment_analyser_tagit-0.6.tar.gz` & `tmp/sentiment_analyser_tagit-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentiment_analyser_tagit-0.6.tar", last modified: Mon Jul 31 04:12:53 2023, max compression
+gzip compressed data, was "sentiment_analyser_tagit-0.7.tar", last modified: Mon Jul 31 04:18:34 2023, max compression
```

## Comparing `sentiment_analyser_tagit-0.6.tar` & `sentiment_analyser_tagit-0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 adithyanarayanan   (501) staff       (20)        0 2023-07-31 04:12:53.976249 sentiment_analyser_tagit-0.6/
--rw-r--r--   0 adithyanarayanan   (501) staff       (20)      207 2023-07-31 04:12:53.976121 sentiment_analyser_tagit-0.6/PKG-INFO
-drwxr-xr-x   0 adithyanarayanan   (501) staff       (20)        0 2023-07-31 04:12:53.975944 sentiment_analyser_tagit-0.6/sentiment_analyser_tagit.egg-info/
--rw-r--r--   0 adithyanarayanan   (501) staff       (20)      207 2023-07-31 04:12:53.000000 sentiment_analyser_tagit-0.6/sentiment_analyser_tagit.egg-info/PKG-INFO
--rw-r--r--   0 adithyanarayanan   (501) staff       (20)      247 2023-07-31 04:12:53.000000 sentiment_analyser_tagit-0.6/sentiment_analyser_tagit.egg-info/SOURCES.txt
--rw-r--r--   0 adithyanarayanan   (501) staff       (20)        1 2023-07-31 04:12:53.000000 sentiment_analyser_tagit-0.6/sentiment_analyser_tagit.egg-info/dependency_links.txt
--rw-r--r--   0 adithyanarayanan   (501) staff       (20)       51 2023-07-31 04:12:53.000000 sentiment_analyser_tagit-0.6/sentiment_analyser_tagit.egg-info/requires.txt
--rw-r--r--   0 adithyanarayanan   (501) staff       (20)        1 2023-07-31 04:12:53.000000 sentiment_analyser_tagit-0.6/sentiment_analyser_tagit.egg-info/top_level.txt
--rw-r--r--   0 adithyanarayanan   (501) staff       (20)       38 2023-07-31 04:12:53.976296 sentiment_analyser_tagit-0.6/setup.cfg
--rw-r--r--   0 adithyanarayanan   (501) staff       (20)      439 2023-07-31 04:12:19.000000 sentiment_analyser_tagit-0.6/setup.py
+drwxr-xr-x   0 adithyanarayanan   (501) staff       (20)        0 2023-07-31 04:18:34.888474 sentiment_analyser_tagit-0.7/
+-rw-r--r--   0 adithyanarayanan   (501) staff       (20)      207 2023-07-31 04:18:34.888345 sentiment_analyser_tagit-0.7/PKG-INFO
+drwxr-xr-x   0 adithyanarayanan   (501) staff       (20)        0 2023-07-31 04:18:34.888142 sentiment_analyser_tagit-0.7/sentiment_analyser_tagit.egg-info/
+-rw-r--r--   0 adithyanarayanan   (501) staff       (20)      207 2023-07-31 04:18:34.000000 sentiment_analyser_tagit-0.7/sentiment_analyser_tagit.egg-info/PKG-INFO
+-rw-r--r--   0 adithyanarayanan   (501) staff       (20)      247 2023-07-31 04:18:34.000000 sentiment_analyser_tagit-0.7/sentiment_analyser_tagit.egg-info/SOURCES.txt
+-rw-r--r--   0 adithyanarayanan   (501) staff       (20)        1 2023-07-31 04:18:34.000000 sentiment_analyser_tagit-0.7/sentiment_analyser_tagit.egg-info/dependency_links.txt
+-rw-r--r--   0 adithyanarayanan   (501) staff       (20)       51 2023-07-31 04:18:34.000000 sentiment_analyser_tagit-0.7/sentiment_analyser_tagit.egg-info/requires.txt
+-rw-r--r--   0 adithyanarayanan   (501) staff       (20)        1 2023-07-31 04:18:34.000000 sentiment_analyser_tagit-0.7/sentiment_analyser_tagit.egg-info/top_level.txt
+-rw-r--r--   0 adithyanarayanan   (501) staff       (20)       38 2023-07-31 04:18:34.888516 sentiment_analyser_tagit-0.7/setup.cfg
+-rw-r--r--   0 adithyanarayanan   (501) staff       (20)      459 2023-07-31 04:18:13.000000 sentiment_analyser_tagit-0.7/setup.py
```

