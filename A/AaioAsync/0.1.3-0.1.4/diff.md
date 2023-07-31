# Comparing `tmp/AaioAsync-0.1.3.tar.gz` & `tmp/AaioAsync-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AaioAsync-0.1.3.tar", last modified: Sat Jul 29 22:37:23 2023, max compression
+gzip compressed data, was "AaioAsync-0.1.4.tar", last modified: Mon Jul 31 10:08:05 2023, max compression
```

## Comparing `AaioAsync-0.1.3.tar` & `AaioAsync-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 22:37:23.990014 AaioAsync-0.1.3/
-drwxrwxrwx   0        0        0        0 2023-07-29 22:37:23.972013 AaioAsync-0.1.3/AaioAsync/
--rw-rw-rw-   0        0        0       26 2023-07-29 17:17:54.000000 AaioAsync-0.1.3/AaioAsync/__init__.py
--rw-rw-rw-   0        0        0     8255 2023-07-29 21:10:19.000000 AaioAsync-0.1.3/AaioAsync/api.py
-drwxrwxrwx   0        0        0        0 2023-07-29 22:37:23.984015 AaioAsync-0.1.3/AaioAsync/exceptions/
--rw-rw-rw-   0        0        0       34 2023-07-29 17:44:03.000000 AaioAsync-0.1.3/AaioAsync/exceptions/__init__.py
--rw-rw-rw-   0        0        0       42 2023-07-29 17:34:35.000000 AaioAsync-0.1.3/AaioAsync/exceptions/errors.py
-drwxrwxrwx   0        0        0        0 2023-07-29 22:37:23.988015 AaioAsync-0.1.3/AaioAsync/models/
--rw-rw-rw-   0        0        0      120 2023-07-27 19:51:43.000000 AaioAsync-0.1.3/AaioAsync/models/balance.py
--rw-rw-rw-   0        0        0      731 2023-07-29 19:20:51.000000 AaioAsync-0.1.3/AaioAsync/models/order.py
--rw-rw-rw-   0        0        0      710 2023-07-29 19:07:16.000000 AaioAsync-0.1.3/AaioAsync/models/withdrawal.py
--rw-rw-rw-   0        0        0     1431 2023-07-29 20:12:10.000000 AaioAsync-0.1.3/AaioAsync/requests.py
-drwxrwxrwx   0        0        0        0 2023-07-29 22:37:23.981015 AaioAsync-0.1.3/AaioAsync.egg-info/
--rw-rw-rw-   0        0        0     1332 2023-07-29 22:37:23.000000 AaioAsync-0.1.3/AaioAsync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-07-29 22:37:23.000000 AaioAsync-0.1.3/AaioAsync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 22:37:23.000000 AaioAsync-0.1.3/AaioAsync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-29 22:37:23.000000 AaioAsync-0.1.3/AaioAsync.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2023-07-29 22:37:23.000000 AaioAsync-0.1.3/AaioAsync.egg-info/requires.txt
--rw-rw-rw-   0        0        0       48 2023-07-29 22:37:23.000000 AaioAsync-0.1.3/AaioAsync.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1332 2023-07-29 22:37:23.990014 AaioAsync-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-29 22:37:23.992015 AaioAsync-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1515 2023-07-29 22:37:18.000000 AaioAsync-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 10:08:05.518648 AaioAsync-0.1.4/
+drwxrwxrwx   0        0        0        0 2023-07-31 10:08:05.499645 AaioAsync-0.1.4/AaioAsync/
+-rw-rw-rw-   0        0        0       26 2023-07-29 17:17:54.000000 AaioAsync-0.1.4/AaioAsync/__init__.py
+-rw-rw-rw-   0        0        0     8225 2023-07-31 09:56:34.000000 AaioAsync-0.1.4/AaioAsync/api.py
+drwxrwxrwx   0        0        0        0 2023-07-31 10:08:05.512646 AaioAsync-0.1.4/AaioAsync/exceptions/
+-rw-rw-rw-   0        0        0       34 2023-07-29 17:44:03.000000 AaioAsync-0.1.4/AaioAsync/exceptions/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-29 17:34:35.000000 AaioAsync-0.1.4/AaioAsync/exceptions/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-31 10:08:05.516647 AaioAsync-0.1.4/AaioAsync/models/
+-rw-rw-rw-   0        0        0      120 2023-07-27 19:51:43.000000 AaioAsync-0.1.4/AaioAsync/models/balance.py
+-rw-rw-rw-   0        0        0      731 2023-07-29 19:20:51.000000 AaioAsync-0.1.4/AaioAsync/models/order.py
+-rw-rw-rw-   0        0        0      710 2023-07-29 19:07:16.000000 AaioAsync-0.1.4/AaioAsync/models/withdrawal.py
+-rw-rw-rw-   0        0        0     1431 2023-07-29 20:12:10.000000 AaioAsync-0.1.4/AaioAsync/requests.py
+drwxrwxrwx   0        0        0        0 2023-07-31 10:08:05.509646 AaioAsync-0.1.4/AaioAsync.egg-info/
+-rw-rw-rw-   0        0        0     1365 2023-07-31 10:08:05.000000 AaioAsync-0.1.4/AaioAsync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-07-31 10:08:05.000000 AaioAsync-0.1.4/AaioAsync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 10:08:05.000000 AaioAsync-0.1.4/AaioAsync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-31 10:08:05.000000 AaioAsync-0.1.4/AaioAsync.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2023-07-31 10:08:05.000000 AaioAsync-0.1.4/AaioAsync.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       48 2023-07-31 10:08:05.000000 AaioAsync-0.1.4/AaioAsync.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1365 2023-07-31 10:08:05.518648 AaioAsync-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-31 10:08:05.519647 AaioAsync-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1569 2023-07-31 10:03:07.000000 AaioAsync-0.1.4/setup.py
```

### Comparing `AaioAsync-0.1.3/AaioAsync/api.py` & `AaioAsync-0.1.4/AaioAsync/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,22 +45,22 @@
 
         Docs: https://wiki.aaio.io/priem-platezhei/sozdanie-zakaza
 
         :param amount: Order amount.
         :param order_id: Order number, which unique in your system, up to 16 characters, without spaces (aA-zZ, 0-9, :, -, _, [, ] , |)
         :param currency: Currency. Default to 'RUB' (RUB, UAH, EUR, USD)
         :param method: Payment Aaio system code name
-        :param desc: Order description. Not working on Aaio side xD
+        :param desc: Order description
         :param email: Buyer mail
         :param lang: Interface language. Default to 'ru' (ru, en)
         :param referal: Referral code
         :param us_key: Parameter that you want to get in the notification"""
 
         if not self.__secretkey or not self._shop:
-            raise Exception('Не указан SecretKey или ShopID.')
+            raise Exception('Не указан SecretKey или ShopID')
 
         params = {
             'merchant_id': self._shop,
             'amount': amount,
             'order_id': order_id.strip(),
             'currency': currency,
             'method': method,
```

### Comparing `AaioAsync-0.1.3/AaioAsync/models/order.py` & `AaioAsync-0.1.4/AaioAsync/models/order.py`

 * *Files identical despite different names*

### Comparing `AaioAsync-0.1.3/AaioAsync/models/withdrawal.py` & `AaioAsync-0.1.4/AaioAsync/models/withdrawal.py`

 * *Files identical despite different names*

### Comparing `AaioAsync-0.1.3/AaioAsync/requests.py` & `AaioAsync-0.1.4/AaioAsync/requests.py`

 * *Files identical despite different names*

### Comparing `AaioAsync-0.1.3/AaioAsync.egg-info/PKG-INFO` & `AaioAsync-0.1.4/AaioAsync.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: AaioAsync
-Version: 0.1.3
+Version: 0.1.4
 Summary: Fully async python wrapper for Aaio.io API
-Home-page: UNKNOWN
+Home-page: https://github.com/Belyashik2K/AaioAsync
 Author: Belyashik2K
 Author-email: lovelybelyashik@gmail.com
 License: Apache License, Version 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # AaioAsync
```

### Comparing `AaioAsync-0.1.3/PKG-INFO` & `AaioAsync-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: AaioAsync
-Version: 0.1.3
+Version: 0.1.4
 Summary: Fully async python wrapper for Aaio.io API
-Home-page: UNKNOWN
+Home-page: https://github.com/Belyashik2K/AaioAsync
 Author: Belyashik2K
 Author-email: lovelybelyashik@gmail.com
 License: Apache License, Version 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # AaioAsync
```

### Comparing `AaioAsync-0.1.3/setup.py` & `AaioAsync-0.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = '0.1.3'
+version = '0.1.4'
 
 setup(name='AaioAsync',
       version=version,
 
       author='Belyashik2K',
       author_email='lovelybelyashik@gmail.com',
 
@@ -56,10 +56,11 @@
 
 ## Docs
 > Go to https://wiki.aaio.io/ for more information about working with acquiring
 """,
       long_description_content_type='text/markdown',
 
       description='Fully async python wrapper for Aaio.io API',
+      url='https://github.com/Belyashik2K/AaioAsync',
       packages=['AaioAsync', 'AaioAsync/exceptions', 'AaioAsync/models'],
       install_requires=['certifi', 'aiohttp', 'pydantic'],
       zip_safe=False)
```

