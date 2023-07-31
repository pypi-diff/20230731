# Comparing `tmp/realtime_twitter_api-0.1.tar.gz` & `tmp/realtime_twitter_api-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "realtime_twitter_api-0.1.tar", last modified: Sun Jul 30 13:26:01 2023, max compression
+gzip compressed data, was "realtime_twitter_api-0.2.tar", last modified: Mon Jul 31 03:49:40 2023, max compression
```

## Comparing `realtime_twitter_api-0.1.tar` & `realtime_twitter_api-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 13:26:01.575423 realtime_twitter_api-0.1/
--rw-rw-rw-   0        0        0       65 2023-07-30 13:26:01.572430 realtime_twitter_api-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2752 2023-07-30 13:21:45.000000 realtime_twitter_api-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 13:26:01.549491 realtime_twitter_api-0.1/realtime_twitter_api/
--rw-rw-rw-   0        0        0     9470 2023-07-30 13:14:15.000000 realtime_twitter_api-0.1/realtime_twitter_api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 13:26:01.568442 realtime_twitter_api-0.1/realtime_twitter_api.egg-info/
--rw-rw-rw-   0        0        0       65 2023-07-30 13:26:01.000000 realtime_twitter_api-0.1/realtime_twitter_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-07-30 13:26:01.000000 realtime_twitter_api-0.1/realtime_twitter_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 13:26:01.000000 realtime_twitter_api-0.1/realtime_twitter_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-30 13:26:01.000000 realtime_twitter_api-0.1/realtime_twitter_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-30 13:26:01.000000 realtime_twitter_api-0.1/realtime_twitter_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 13:26:01.576419 realtime_twitter_api-0.1/setup.cfg
--rw-rw-rw-   0        0        0      179 2023-07-30 13:25:21.000000 realtime_twitter_api-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 03:49:40.538138 realtime_twitter_api-0.2/
+-rw-rw-rw-   0        0        0       65 2023-07-31 03:49:40.536139 realtime_twitter_api-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2752 2023-07-30 13:21:45.000000 realtime_twitter_api-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 03:49:40.514204 realtime_twitter_api-0.2/realtime_twitter_api/
+-rw-rw-rw-   0        0        0     9467 2023-07-31 03:47:20.000000 realtime_twitter_api-0.2/realtime_twitter_api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 03:49:40.533147 realtime_twitter_api-0.2/realtime_twitter_api.egg-info/
+-rw-rw-rw-   0        0        0       65 2023-07-31 03:49:40.000000 realtime_twitter_api-0.2/realtime_twitter_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-07-31 03:49:40.000000 realtime_twitter_api-0.2/realtime_twitter_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 03:49:40.000000 realtime_twitter_api-0.2/realtime_twitter_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 03:49:40.000000 realtime_twitter_api-0.2/realtime_twitter_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-31 03:49:40.000000 realtime_twitter_api-0.2/realtime_twitter_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 03:49:40.539131 realtime_twitter_api-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      179 2023-07-31 03:45:06.000000 realtime_twitter_api-0.2/setup.py
```

### Comparing `realtime_twitter_api-0.1/README.md` & `realtime_twitter_api-0.2/README.md`

 * *Files identical despite different names*

### Comparing `realtime_twitter_api-0.1/realtime_twitter_api/__init__.py` & `realtime_twitter_api-0.2/realtime_twitter_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         self.id = tweet_data['id']
         self.verified = tweet_data['verified']
         self.urls = [url['expandedUrl'] for url in tweet_data['urls']]
         self.hashtags = [hashtag['text'] for hashtag in tweet_data['hashtags']]
         self.mentions = [mention['id'] for mention in tweet_data['mentions']]
         self.created_at = tweet_data['createdAt']
         self.reply_count = tweet_data['replyCount']
-        self.rt_count = tweet_data['replyCount']
+        self.rt_count = tweet_data['rtCount']
         self.likes_count = tweet_data['likesCount']
         self.user_id = tweet_data['userId']
         self.user_name = tweet_data['name']
         self.user_screen_name = tweet_data['screenName']
         self.quoted_tweet = tweet_data.get('quotedTweet') and tweet_data['quotedTweet']['url'].split('?')[0]
 
         self.media = [
```

