# Comparing `tmp/adafri-0.0.70.tar.gz` & `tmp/adafri-0.0.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.70.tar", last modified: Fri Jul 28 08:15:18 2023, max compression
+gzip compressed data, was "adafri-0.0.71.tar", last modified: Mon Jul 31 02:28:15 2023, max compression
```

## Comparing `adafri-0.0.70.tar` & `adafri-0.0.71.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.177224 adafri-0.0.70/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-28 08:15:18.176752 adafri-0.0.70/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.133098 adafri-0.0.70/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-28 08:15:10.000000 adafri-0.0.70/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.141056 adafri-0.0.70/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.70/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.70/adafri/utils/country.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.70/adafri/utils/phone_number.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.70/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    18952 2023-07-28 07:08:29.000000 adafri-0.0.70/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.142500 adafri-0.0.70/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.70/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.143558 adafri-0.0.70/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.70/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.146522 adafri-0.0.70/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.70/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.70/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3852 2023-07-28 08:14:22.000000 adafri-0.0.70/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.147292 adafri-0.0.70/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.70/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.149399 adafri-0.0.70/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.70/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-26 04:56:41.000000 adafri-0.0.70/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.150700 adafri-0.0.70/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.70/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.151177 adafri-0.0.70/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      933 2023-07-28 08:08:06.000000 adafri-0.0.70/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.165974 adafri-0.0.70/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.70/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6973 2023-07-28 05:09:47.000000 adafri-0.0.70/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5478 2023-07-28 08:09:48.000000 adafri-0.0.70/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6304 2023-07-28 07:52:06.000000 adafri-0.0.70/adafri/v1/auth/oauth/models/code.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2444 2023-07-28 08:09:16.000000 adafri-0.0.70/adafri/v1/auth/oauth/models/code_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    16141 2023-07-28 06:11:41.000000 adafri-0.0.70/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3653 2023-07-28 08:10:56.000000 adafri-0.0.70/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9462 2023-07-26 05:24:58.000000 adafri-0.0.70/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3728 2023-07-28 08:11:40.000000 adafri-0.0.70/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.168950 adafri-0.0.70/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.70/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.70/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.70/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.171204 adafri-0.0.70/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.70/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.70/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.171919 adafri-0.0.70/adafri/v1/mailing/
--rw-r--r--   0 ibrahima   (502) staff       (20)     7392 2023-07-26 04:34:01.000000 adafri-0.0.70/adafri/v1/mailing/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.172893 adafri-0.0.70/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.70/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.175933 adafri-0.0.70/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.70/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    11624 2023-07-26 07:42:34.000000 adafri-0.0.70/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     7382 2023-07-28 08:13:51.000000 adafri-0.0.70/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-28 08:15:18.135467 adafri-0.0.70/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-28 08:15:18.000000 adafri-0.0.70/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1329 2023-07-28 08:15:18.000000 adafri-0.0.70/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-28 08:15:18.000000 adafri-0.0.70/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-28 08:15:18.000000 adafri-0.0.70/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-28 08:15:18.177489 adafri-0.0.70/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.70/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.030449 adafri-0.0.71/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-31 02:28:15.029816 adafri-0.0.71/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:14.979828 adafri-0.0.71/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-31 02:28:02.000000 adafri-0.0.71/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:14.995497 adafri-0.0.71/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.71/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.71/adafri/utils/country.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.71/adafri/utils/phone_number.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1356 2023-07-31 01:55:04.000000 adafri-0.0.71/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    19150 2023-07-31 02:21:52.000000 adafri-0.0.71/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:14.996374 adafri-0.0.71/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.71/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:14.997445 adafri-0.0.71/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.71/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.000902 adafri-0.0.71/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.71/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.71/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3852 2023-07-28 08:14:22.000000 adafri-0.0.71/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.001886 adafri-0.0.71/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.71/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.003708 adafri-0.0.71/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.71/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-26 04:56:41.000000 adafri-0.0.71/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.005063 adafri-0.0.71/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.71/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.005839 adafri-0.0.71/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      965 2023-07-28 08:17:28.000000 adafri-0.0.71/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.016964 adafri-0.0.71/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.71/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6979 2023-07-31 01:04:15.000000 adafri-0.0.71/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5478 2023-07-28 08:09:48.000000 adafri-0.0.71/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6529 2023-07-31 01:47:56.000000 adafri-0.0.71/adafri/v1/auth/oauth/models/code.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2505 2023-07-31 01:28:33.000000 adafri-0.0.71/adafri/v1/auth/oauth/models/code_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    16147 2023-07-31 01:04:27.000000 adafri-0.0.71/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3653 2023-07-28 08:10:56.000000 adafri-0.0.71/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9468 2023-07-31 01:04:45.000000 adafri-0.0.71/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3728 2023-07-28 08:11:40.000000 adafri-0.0.71/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.020739 adafri-0.0.71/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.71/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.71/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.71/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.023157 adafri-0.0.71/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.71/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.71/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.023954 adafri-0.0.71/adafri/v1/mailing/
+-rw-r--r--   0 ibrahima   (502) staff       (20)    11306 2023-07-31 02:27:42.000000 adafri-0.0.71/adafri/v1/mailing/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.024781 adafri-0.0.71/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.71/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:15.028205 adafri-0.0.71/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.71/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    11624 2023-07-26 07:42:34.000000 adafri-0.0.71/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     7382 2023-07-28 08:13:51.000000 adafri-0.0.71/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-31 02:28:14.989522 adafri-0.0.71/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-31 02:28:14.000000 adafri-0.0.71/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1329 2023-07-31 02:28:14.000000 adafri-0.0.71/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-31 02:28:14.000000 adafri-0.0.71/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-31 02:28:14.000000 adafri-0.0.71/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-31 02:28:15.030810 adafri-0.0.71/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.71/setup.py
```

### Comparing `adafri-0.0.70/adafri/utils/country.py` & `adafri-0.0.71/adafri/utils/country.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.70/adafri/utils/phone_number.py` & `adafri-0.0.71/adafri/utils/phone_number.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.70/adafri/utils/response.py` & `adafri-0.0.71/adafri/utils/response.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,21 +12,24 @@
     status_200 = 200
     status_400 = 400
 
 @dataclass
 class Error:
     message: str
     name: str
-    error_code: int
+    error_code: int = 1
 
     @staticmethod
     def from_dict(obj: Any) -> 'Error':
         _message = str(obj.get("message"))
         _name = str(obj.get("name"))
-        _error_code = int(obj.get("error_code"))
+        _error_code = "1"
+        code = obj.get("error_code")
+        if code is not None:
+            _error_code = int(str(code))
         return Error(_message, _name, _error_code)
 
 @dataclass
 class ApiResponse:
     status: str
     status_code: int
     data: Any
```

### Comparing `adafri-0.0.70/adafri/utils/utils.py` & `adafri-0.0.71/adafri/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,24 @@
 ENCRYPTION_KEY = base64.b64encode(hash.hexdigest()[:32].encode()).decode();
 
 
 camel_pat = re.compile(r'([A-Z])')
 under_pat = re.compile(r'_([a-z])')
 
 
+def boolean(data):
+    if type(data) is bool:
+        return data;
+    if type(data) is str:
+        if data.lower() == 'true':
+            return True;
+        if data.lower() == 'false':
+            return False;
+    return None;
+
 class Object:
     def __init__(self, **kwargs):
         if kwargs is not None:
             for k, v in kwargs.items():
                 setattr(self, k, v);
 
 def split_by_crlf(s):
@@ -312,15 +322,14 @@
     
     @staticmethod
     def merge_dict(current_dict, target_dict):
         final_dict = target_dict
         for key in pydash.keys(current_dict):
             if key not in final_dict or bool(final_dict[key]) is False or type(current_dict[key])!=type(final_dict[key]) or final_dict[key]!=current_dict[key]:
                 final_dict[key] = current_dict[key]
-        print('final', final_dict)
         return final_dict;
 
     @staticmethod
     def string_to_json(element):
         try:
             return json.loads(element);
         except Exception as e:
```

### Comparing `adafri-0.0.70/adafri/v1/account/models/account.py` & `adafri-0.0.71/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.70/adafri/v1/account/models/account_fields.py` & `adafri-0.0.71/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.70/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.71/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.70/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.71/adafri/v1/auth/oauth/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,9 +8,10 @@
 from .models.grant import (OAuthGrant, AuthorizationCodeGrant, OpenIDCode, OpenIDImplicitGrant, OpenIDHybridGrant, OpenIDAuthorizationCodeGrant)
 from .models import token
 from .models import token_fields
 from .models.token_fields import (TokenFieldsProps, TokenFields)
 from .models.token import (OAuthToken, TokenGenerator, TokenValidator, RefreshTokenGrant, TokenRevocationEndpoint)
 from .models import code
 from .models import code_fields
+from .models.code import (Code)
 from .models.code_fields import (CodeFieldsProps, CodeFields)
 from .server import (oidc_authorization_server, authorization_server, require_oauth, require_oidc_oauth, config_oauth, config_oidc_oauth)
```

### Comparing `adafri-0.0.70/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.71/adafri/v1/auth/oauth/models/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     def getOAuthClient(self) -> 'OAuthClient':
         if bool(self.id):
             doc = self.document_reference().get();
             if doc.exists is False:
                 return None;
             return OAuthClient.from_dict(doc.to_dict(), db=self.db, collection_name=self.collection_name);
         if bool(self.client_id):
-            return self.query([{"key": ClientFields.client_id, "comp": "==", "value": self.client_id}])
+            return self.query([{"key": ClientFields.client_id, "comp": "==", "value": self.client_id}], True)
 
     @staticmethod
     def generate(**kwargs) -> 'ApiResponse':
         data_dict = DictUtils.pick_fields(kwargs, ClientFields.filtered_keys('mutable', True));
         client_model = OAuthClient.from_dict(DictUtils.merge_dict(data_dict, OAuthClient.generate_model()));
         
         if bool(client_model.to_json()) is False:
```

### Comparing `adafri-0.0.70/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.71/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.70/adafri/v1/auth/oauth/models/code.py` & `adafri-0.0.71/adafri/v1/auth/oauth/models/code.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     target: str
     code_type: str
     createdAt: any
     expired_at: str
     expires_in: int
 
     def __init__(self, code=None, **kwargs):
-        if type(token) is str:
-            token = {"access_token": token} 
-        (cls_object, keys, data_args) = init_class_kwargs(self, token, STANDARD_FIELDS, CodeFieldsProps, CODE_COLLECTION, ['id'], **kwargs)
+        if type(code) is str or type(code) is int:
+            code = {"code": str(code), "code_type": "email_validation"} 
+        (cls_object, keys, data_args) = init_class_kwargs(self, code, STANDARD_FIELDS, CodeFieldsProps, CODE_COLLECTION, ['id'], **kwargs)
         super().__init__(**data_args);
         for key in keys:
             setattr(self, key, cls_object[key]) 
 
 
     @staticmethod
     def generate_model(_key_="default_value"):
@@ -39,31 +39,33 @@
         return _client
 
     def query(self, query_params: list, first=False, limit=None):
         result = [];
         query_result = self.custom_query(query_params, first=first, limit=limit)
         if bool(query_result):
             if first is True:
-                return Code.from_dict(token=query_result, db=self.db, collection_name=self.collection_name)
+                return Code.from_dict(code=query_result, db=self.db, collection_name=self.collection_name)
             else:
                 for doc in query_result:
-                    result.append(Code.from_dict(token=doc, db=self.db, collection_name=self.collection_name))
+                    result.append(Code.from_dict(code=doc, db=self.db, collection_name=self.collection_name))
                 return result
         if first:
                 return None
         return [];
 
     def getCode(self) -> 'Code':
         if bool(self.id):
             doc = self.document_reference().get();
             if doc.exists is False:
                 return None;
             return Code.from_dict(doc.to_dict(), db=self.db, collection_name=self.collection_name);
-        if bool(self.code):
-            return self.query([{"key": CodeFields.code, "comp": "==", "value": self.code}])
+        if bool(self.code) and bool(self.code_type):
+            params = [{"key": CodeFields.code, "comp": "==", "value": self.code}, {"key": CodeFields.code_type, "comp": "==", "value": self.code_type}]
+            return self.query(params, True)
+        return None;
 
     @staticmethod
     def generate(**kwargs) -> 'ApiResponse':
         data_dict = DictUtils.pick_fields(kwargs, CodeFields.filtered_keys('pickable', True));
         code_model = Code.from_dict(DictUtils.merge_dict(data_dict, Code.generate_model()));
         
         if bool(code_model.to_json()) is False:
@@ -106,25 +108,25 @@
             print(e)
             return None;
     
     def use_code(self):
         code = self.getCode();
         if code is None:
             return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"Invalid code","INVALID_REQUEST", 1));
-        remove = self.remove()
-        if remove.status == ResponseStatus.ERROR:
-            return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"An error occurated","INVALID_REQUEST", 1));
         if code.is_expired():
             return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"Expired code","INVALID_REQUEST", 1));
-        return ApiResponse(ResponseStatus.OK, StatusCode.status_200, {"message": "success"});
+        remove = code.remove()
+        if remove.status == ResponseStatus.ERROR:
+            return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"An error occurated","INVALID_REQUEST", 1));
+        return ApiResponse(ResponseStatus.OK, StatusCode.status_200, {"message": "success"}, None);
 
     def remove(self):
         try:
             if self.id is None:
                 return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"Cannot identify Authorization code with id {self.id} to delete","INVALID_REQUEST", 1));
             deleted = self.document_reference().delete();
             return ApiResponse(ResponseStatus.OK, StatusCode.status_200, {"message": f"Code {self.id} deleted"}, None);
-        except:
-            return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"An error occurated while removing authorization code with id {self.id}","INVALID_REQUEST", 1));
+        except Exception as e:
+            return ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error(f"An error occurated while removing authorization code with id {self.id} {str(e)}","INVALID_REQUEST", 1));
 
     def is_expired(self):
         return is_expired(self.expired_at)
```

### Comparing `adafri-0.0.70/adafri/v1/auth/oauth/models/code_fields.py` & `adafri-0.0.71/adafri/v1/auth/oauth/models/code_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,8 +94,9 @@
         "editable": False,
         "interactive": True,
         "default_value": get_code_expire_at(900).isoformat(),
         "pickable": True
     },
 
     
-}
+}
+STANDARD_FIELDS = CodeFields.filtered_keys('pickable', True)
```

### Comparing `adafri-0.0.70/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.71/adafri/v1/auth/oauth/models/grant.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     def getOAuthGrant(self) -> 'OAuthGrant':
         if bool(self.id):
             doc = self.document_reference(self.id).get();
             if doc.exists is False:
                 return None;
             return OAuthGrant.from_dict(doc.to_dict(), db=self.db, collection_name=self.collection_name);
         if bool(self.code):
-            return self.query([{"key": GrantFields.code, "comp": "==", "value": self.code}])
+            return self.query([{"key": GrantFields.code, "comp": "==", "value": self.code}], True)
 
     @staticmethod
     def generate(**kwargs) -> 'ApiResponse':
         data_dict = DictUtils.pick_fields(kwargs, GrantFields.filtered_keys('mutable', True));
         authorization_code_model = OAuthGrant.from_dict(DictUtils.merge_dict(data_dict, OAuthGrant.generate_model()));
         
         if bool(authorization_code_model.to_json()) is False:
```

### Comparing `adafri-0.0.70/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.71/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.70/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.71/adafri/v1/auth/oauth/models/token.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     def getOAuthToken(self) -> 'OAuthToken':
         if bool(self.id):
             doc = self.document_reference().get();
             if doc.exists is False:
                 return None;
             return OAuthToken.from_dict(doc.to_dict(), db=self.db, collection_name=self.collection_name);
         if bool(self.access_token):
-            return self.query([{"key": TokenFields.access_token, "comp": "==", "value": self.access_token}])
+            return self.query([{"key": TokenFields.access_token, "comp": "==", "value": self.access_token}], True)
 
     @staticmethod
     def generate(**kwargs) -> 'ApiResponse':
         data_dict = DictUtils.pick_fields(kwargs, TokenFields.filtered_keys('pickable', True));
         token_model = OAuthToken.from_dict(DictUtils.merge_dict(data_dict, OAuthToken.generate_model()));
         
         if bool(token_model.to_json()) is False:
```

### Comparing `adafri-0.0.70/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.71/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.70/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.71/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.70/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.71/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.70/adafri/v1/base/firebase_collection.py` & `adafri-0.0.71/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.70/adafri/v1/user/models/user.py` & `adafri-0.0.71/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.70/adafri/v1/user/models/user_fields.py` & `adafri-0.0.71/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.70/adafri.egg-info/SOURCES.txt` & `adafri-0.0.71/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.70/setup.py` & `adafri-0.0.71/setup.py`

 * *Files identical despite different names*

