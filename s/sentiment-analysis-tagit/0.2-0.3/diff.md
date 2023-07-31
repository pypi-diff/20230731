# Comparing `tmp/sentiment-analysis-tagit-0.2.tar.gz` & `tmp/sentiment-analysis-tagit-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentiment-analysis-tagit-0.2.tar", last modified: Mon Jul 31 03:59:42 2023, max compression
+gzip compressed data, was "sentiment-analysis-tagit-0.3.tar", last modified: Mon Jul 31 04:00:31 2023, max compression
```

## Comparing `sentiment-analysis-tagit-0.2.tar` & `sentiment-analysis-tagit-0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 adithyanarayanan   (501) staff       (20)        0 2023-07-31 03:59:42.684897 sentiment-analysis-tagit-0.2/
--rw-r--r--   0 adithyanarayanan   (501) staff       (20)      207 2023-07-31 03:59:42.684766 sentiment-analysis-tagit-0.2/PKG-INFO
-drwxr-xr-x   0 adithyanarayanan   (501) staff       (20)        0 2023-07-31 03:59:42.684581 sentiment-analysis-tagit-0.2/sentiment_analysis_tagit.egg-info/
--rw-r--r--   0 adithyanarayanan   (501) staff       (20)      207 2023-07-31 03:59:42.000000 sentiment-analysis-tagit-0.2/sentiment_analysis_tagit.egg-info/PKG-INFO
--rw-r--r--   0 adithyanarayanan   (501) staff       (20)      247 2023-07-31 03:59:42.000000 sentiment-analysis-tagit-0.2/sentiment_analysis_tagit.egg-info/SOURCES.txt
--rw-r--r--   0 adithyanarayanan   (501) staff       (20)        1 2023-07-31 03:59:42.000000 sentiment-analysis-tagit-0.2/sentiment_analysis_tagit.egg-info/dependency_links.txt
--rw-r--r--   0 adithyanarayanan   (501) staff       (20)       51 2023-07-31 03:59:42.000000 sentiment-analysis-tagit-0.2/sentiment_analysis_tagit.egg-info/requires.txt
--rw-r--r--   0 adithyanarayanan   (501) staff       (20)        1 2023-07-31 03:59:42.000000 sentiment-analysis-tagit-0.2/sentiment_analysis_tagit.egg-info/top_level.txt
--rw-r--r--   0 adithyanarayanan   (501) staff       (20)       38 2023-07-31 03:59:42.684941 sentiment-analysis-tagit-0.2/setup.cfg
--rw-r--r--   0 adithyanarayanan   (501) staff       (20)      439 2023-07-31 03:59:40.000000 sentiment-analysis-tagit-0.2/setup.py
+drwxr-xr-x   0 adithyanarayanan   (501) staff       (20)        0 2023-07-31 04:00:31.629206 sentiment-analysis-tagit-0.3/
+-rw-r--r--   0 adithyanarayanan   (501) staff       (20)      207 2023-07-31 04:00:31.629057 sentiment-analysis-tagit-0.3/PKG-INFO
+drwxr-xr-x   0 adithyanarayanan   (501) staff       (20)        0 2023-07-31 04:00:31.628755 sentiment-analysis-tagit-0.3/sentiment_analysis_tagit.egg-info/
+-rw-r--r--   0 adithyanarayanan   (501) staff       (20)      207 2023-07-31 04:00:31.000000 sentiment-analysis-tagit-0.3/sentiment_analysis_tagit.egg-info/PKG-INFO
+-rw-r--r--   0 adithyanarayanan   (501) staff       (20)      247 2023-07-31 04:00:31.000000 sentiment-analysis-tagit-0.3/sentiment_analysis_tagit.egg-info/SOURCES.txt
+-rw-r--r--   0 adithyanarayanan   (501) staff       (20)        1 2023-07-31 04:00:31.000000 sentiment-analysis-tagit-0.3/sentiment_analysis_tagit.egg-info/dependency_links.txt
+-rw-r--r--   0 adithyanarayanan   (501) staff       (20)       51 2023-07-31 04:00:31.000000 sentiment-analysis-tagit-0.3/sentiment_analysis_tagit.egg-info/requires.txt
+-rw-r--r--   0 adithyanarayanan   (501) staff       (20)        1 2023-07-31 04:00:31.000000 sentiment-analysis-tagit-0.3/sentiment_analysis_tagit.egg-info/top_level.txt
+-rw-r--r--   0 adithyanarayanan   (501) staff       (20)       38 2023-07-31 04:00:31.629247 sentiment-analysis-tagit-0.3/setup.cfg
+-rw-r--r--   0 adithyanarayanan   (501) staff       (20)      439 2023-07-31 04:00:27.000000 sentiment-analysis-tagit-0.3/setup.py
```

