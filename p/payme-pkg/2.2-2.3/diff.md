# Comparing `tmp/payme-pkg-2.2.tar.gz` & `tmp/payme-pkg-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/payme-pkg-2.2.tar", last modified: Sun Apr 23 09:45:13 2023, max compression
+gzip compressed data, was "payme-pkg-2.3.tar", last modified: Mon Jul 31 07:04:07 2023, max compression
```

## Comparing `payme-pkg-2.2.tar` & `payme-pkg-2.3.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-04-23 09:45:13.000000 payme-pkg-2.2/
--rw-r--r--   0 thenight   (501) staff       (20)      338 2023-04-23 09:45:13.000000 payme-pkg-2.2/PKG-INFO
--rw-r--r--   0 thenight   (501) staff       (20)    19593 2023-04-23 09:08:57.000000 payme-pkg-2.2/README.md
--rw-r--r--   0 thenight   (501) staff       (20)      538 2023-04-23 09:44:11.000000 payme-pkg-2.2/setup.py
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-04-23 09:45:13.000000 payme-pkg-2.2/lib/
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-04-23 09:45:13.000000 payme-pkg-2.2/lib/payme_pkg.egg-info/
--rw-r--r--   0 thenight   (501) staff       (20)      338 2023-04-23 09:45:12.000000 payme-pkg-2.2/lib/payme_pkg.egg-info/PKG-INFO
--rw-r--r--   0 thenight   (501) staff       (20)     1097 2023-04-23 09:45:12.000000 payme-pkg-2.2/lib/payme_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 thenight   (501) staff       (20)       59 2023-04-23 09:45:12.000000 payme-pkg-2.2/lib/payme_pkg.egg-info/requires.txt
--rw-r--r--   0 thenight   (501) staff       (20)        6 2023-04-23 09:45:12.000000 payme-pkg-2.2/lib/payme_pkg.egg-info/top_level.txt
--rw-r--r--   0 thenight   (501) staff       (20)        1 2023-04-23 09:45:12.000000 payme-pkg-2.2/lib/payme_pkg.egg-info/dependency_links.txt
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-04-23 09:45:13.000000 payme-pkg-2.2/lib/payme/
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-04-23 09:45:13.000000 payme-pkg-2.2/lib/payme/receipts/
--rw-r--r--   0 thenight   (501) staff       (20)     6616 2023-04-19 14:50:57.000000 payme-pkg-2.2/lib/payme/receipts/subscribe_receipts.py
--rw-r--r--   0 thenight   (501) staff       (20)       32 2023-04-19 09:04:54.000000 payme-pkg-2.2/lib/payme/receipts/__init__.py
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-04-23 09:45:13.000000 payme-pkg-2.2/lib/payme/migrations/
--rw-r--r--   0 thenight   (501) staff       (20)        0 2023-04-19 08:59:40.000000 payme-pkg-2.2/lib/payme/migrations/__init__.py
--rw-r--r--   0 thenight   (501) staff       (20)     2061 2023-04-19 08:59:33.000000 payme-pkg-2.2/lib/payme/migrations/0001_initial.py
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-04-23 09:45:13.000000 payme-pkg-2.2/lib/payme/methods/
--rw-r--r--   0 thenight   (501) staff       (20)      708 2023-04-19 05:54:29.000000 payme-pkg-2.2/lib/payme/methods/check_perform_transaction.py
--rw-r--r--   0 thenight   (501) staff       (20)     1847 2023-04-19 15:06:51.000000 payme-pkg-2.2/lib/payme/methods/cancel_transaction.py
--rw-r--r--   0 thenight   (501) staff       (20)     2302 2023-04-19 06:34:08.000000 payme-pkg-2.2/lib/payme/methods/create_transaction.py
--rw-r--r--   0 thenight   (501) staff       (20)     1538 2023-04-19 07:34:08.000000 payme-pkg-2.2/lib/payme/methods/perform_transaction.py
--rw-r--r--   0 thenight   (501) staff       (20)        0 2023-04-18 15:23:39.000000 payme-pkg-2.2/lib/payme/methods/__init__.py
--rw-r--r--   0 thenight   (501) staff       (20)     1954 2023-04-19 07:14:23.000000 payme-pkg-2.2/lib/payme/methods/generate_link.py
--rw-r--r--   0 thenight   (501) staff       (20)     1424 2023-04-19 15:07:40.000000 payme-pkg-2.2/lib/payme/methods/check_transaction.py
--rw-r--r--   0 thenight   (501) staff       (20)     1974 2023-04-23 09:30:02.000000 payme-pkg-2.2/lib/payme/models.py
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-04-23 09:45:13.000000 payme-pkg-2.2/lib/payme/decorators/
--rw-r--r--   0 thenight   (501) staff       (20)        0 2023-04-19 13:55:21.000000 payme-pkg-2.2/lib/payme/decorators/__init__.py
--rw-r--r--   0 thenight   (501) staff       (20)      908 2023-04-19 16:14:02.000000 payme-pkg-2.2/lib/payme/decorators/decorators.py
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-04-23 09:45:13.000000 payme-pkg-2.2/lib/payme/cards/
--rw-r--r--   0 thenight   (501) staff       (20)     5071 2023-04-19 16:17:49.000000 payme-pkg-2.2/lib/payme/cards/subscribe_cards.py
--rw-r--r--   0 thenight   (501) staff       (20)       29 2023-04-18 16:06:59.000000 payme-pkg-2.2/lib/payme/cards/__init__.py
--rw-r--r--   0 thenight   (501) staff       (20)     2588 2023-04-19 16:07:41.000000 payme-pkg-2.2/lib/payme/serializers.py
--rw-r--r--   0 thenight   (501) staff       (20)        0 2023-04-19 11:31:50.000000 payme-pkg-2.2/lib/payme/__init__.py
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-04-23 09:45:13.000000 payme-pkg-2.2/lib/payme/utils/
--rw-r--r--   0 thenight   (501) staff       (20)      186 2023-04-19 17:04:27.000000 payme-pkg-2.2/lib/payme/utils/logging.py
--rw-r--r--   0 thenight   (501) staff       (20)      209 2023-04-18 15:23:39.000000 payme-pkg-2.2/lib/payme/utils/support.py
--rw-r--r--   0 thenight   (501) staff       (20)        0 2023-04-18 15:23:39.000000 payme-pkg-2.2/lib/payme/utils/__init__.py
--rw-r--r--   0 thenight   (501) staff       (20)      236 2023-04-19 13:45:21.000000 payme-pkg-2.2/lib/payme/utils/to_json.py
--rw-r--r--   0 thenight   (501) staff       (20)      680 2023-04-18 15:23:39.000000 payme-pkg-2.2/lib/payme/utils/get_params.py
--rw-r--r--   0 thenight   (501) staff       (20)      264 2023-04-18 19:19:38.000000 payme-pkg-2.2/lib/payme/apps.py
--rw-r--r--   0 thenight   (501) staff       (20)      287 2023-04-23 08:58:58.000000 payme-pkg-2.2/lib/payme/admin.py
-drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-04-23 09:45:13.000000 payme-pkg-2.2/lib/payme/errors/
--rw-r--r--   0 thenight   (501) staff       (20)        0 2023-04-18 15:23:39.000000 payme-pkg-2.2/lib/payme/errors/__init__.py
--rw-r--r--   0 thenight   (501) staff       (20)     2241 2023-04-19 05:45:54.000000 payme-pkg-2.2/lib/payme/errors/exceptions.py
--rw-r--r--   0 thenight   (501) staff       (20)      139 2023-04-18 15:23:39.000000 payme-pkg-2.2/lib/payme/urls.py
--rw-r--r--   0 thenight   (501) staff       (20)     4370 2023-04-19 13:41:19.000000 payme-pkg-2.2/lib/payme/views.py
--rw-r--r--   0 thenight   (501) staff       (20)      107 2023-04-23 09:45:13.000000 payme-pkg-2.2/setup.cfg
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-07-31 07:04:07.223381 payme-pkg-2.3/
+-rw-r--r--   0 thenight   (501) staff       (20)     1062 2023-07-29 22:54:03.000000 payme-pkg-2.3/LICENSE.txt
+-rw-r--r--   0 thenight   (501) staff       (20)      338 2023-07-31 07:04:07.223698 payme-pkg-2.3/PKG-INFO
+-rw-r--r--   0 thenight   (501) staff       (20)    19766 2023-07-29 22:54:03.000000 payme-pkg-2.3/README.md
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-07-31 07:04:07.177690 payme-pkg-2.3/lib/
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-07-31 07:04:07.187768 payme-pkg-2.3/lib/payme/
+-rw-r--r--   0 thenight   (501) staff       (20)        0 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/__init__.py
+-rw-r--r--   0 thenight   (501) staff       (20)      287 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/admin.py
+-rw-r--r--   0 thenight   (501) staff       (20)      264 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/apps.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-07-31 07:04:07.189913 payme-pkg-2.3/lib/payme/cards/
+-rw-r--r--   0 thenight   (501) staff       (20)       29 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/cards/__init__.py
+-rw-r--r--   0 thenight   (501) staff       (20)     5071 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/cards/subscribe_cards.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-07-31 07:04:07.191569 payme-pkg-2.3/lib/payme/decorators/
+-rw-r--r--   0 thenight   (501) staff       (20)        0 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/decorators/__init__.py
+-rw-r--r--   0 thenight   (501) staff       (20)      908 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/decorators/decorators.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-07-31 07:04:07.193338 payme-pkg-2.3/lib/payme/errors/
+-rw-r--r--   0 thenight   (501) staff       (20)        0 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/errors/__init__.py
+-rw-r--r--   0 thenight   (501) staff       (20)     2241 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/errors/exceptions.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-07-31 07:04:07.201867 payme-pkg-2.3/lib/payme/methods/
+-rw-r--r--   0 thenight   (501) staff       (20)        0 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/methods/__init__.py
+-rw-r--r--   0 thenight   (501) staff       (20)     1847 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/methods/cancel_transaction.py
+-rw-r--r--   0 thenight   (501) staff       (20)      708 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/methods/check_perform_transaction.py
+-rw-r--r--   0 thenight   (501) staff       (20)     1423 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/methods/check_transaction.py
+-rw-r--r--   0 thenight   (501) staff       (20)     2302 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/methods/create_transaction.py
+-rw-r--r--   0 thenight   (501) staff       (20)     1954 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/methods/generate_link.py
+-rw-r--r--   0 thenight   (501) staff       (20)     2124 2023-07-31 06:55:26.000000 payme-pkg-2.3/lib/payme/methods/get_statement.py
+-rw-r--r--   0 thenight   (501) staff       (20)     1538 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/methods/perform_transaction.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-07-31 07:04:07.204947 payme-pkg-2.3/lib/payme/migrations/
+-rw-r--r--   0 thenight   (501) staff       (20)     2061 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/migrations/0001_initial.py
+-rw-r--r--   0 thenight   (501) staff       (20)        0 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/migrations/__init__.py
+-rw-r--r--   0 thenight   (501) staff       (20)     1974 2023-07-31 07:00:59.000000 payme-pkg-2.3/lib/payme/models.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-07-31 07:04:07.207297 payme-pkg-2.3/lib/payme/receipts/
+-rw-r--r--   0 thenight   (501) staff       (20)       32 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/receipts/__init__.py
+-rw-r--r--   0 thenight   (501) staff       (20)     6616 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/receipts/subscribe_receipts.py
+-rw-r--r--   0 thenight   (501) staff       (20)     2755 2023-07-31 06:55:26.000000 payme-pkg-2.3/lib/payme/serializers.py
+-rw-r--r--   0 thenight   (501) staff       (20)      139 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/urls.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-07-31 07:04:07.217743 payme-pkg-2.3/lib/payme/utils/
+-rw-r--r--   0 thenight   (501) staff       (20)        0 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/utils/__init__.py
+-rw-r--r--   0 thenight   (501) staff       (20)      719 2023-07-31 06:55:26.000000 payme-pkg-2.3/lib/payme/utils/get_params.py
+-rw-r--r--   0 thenight   (501) staff       (20)      186 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/utils/logging.py
+-rw-r--r--   0 thenight   (501) staff       (20)      546 2023-07-31 06:55:26.000000 payme-pkg-2.3/lib/payme/utils/make_aware_datetime.py
+-rw-r--r--   0 thenight   (501) staff       (20)      209 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/utils/support.py
+-rw-r--r--   0 thenight   (501) staff       (20)      236 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/utils/to_json.py
+-rw-r--r--   0 thenight   (501) staff       (20)     4492 2023-07-29 22:54:03.000000 payme-pkg-2.3/lib/payme/views.py
+drwxr-xr-x   0 thenight   (501) staff       (20)        0 2023-07-31 07:04:07.222764 payme-pkg-2.3/lib/payme_pkg.egg-info/
+-rw-r--r--   0 thenight   (501) staff       (20)      338 2023-07-31 07:04:07.000000 payme-pkg-2.3/lib/payme_pkg.egg-info/PKG-INFO
+-rw-r--r--   0 thenight   (501) staff       (20)     1183 2023-07-31 07:04:07.000000 payme-pkg-2.3/lib/payme_pkg.egg-info/SOURCES.txt
+-rw-r--r--   0 thenight   (501) staff       (20)        1 2023-07-31 07:04:07.000000 payme-pkg-2.3/lib/payme_pkg.egg-info/dependency_links.txt
+-rw-r--r--   0 thenight   (501) staff       (20)       59 2023-07-31 07:04:07.000000 payme-pkg-2.3/lib/payme_pkg.egg-info/requires.txt
+-rw-r--r--   0 thenight   (501) staff       (20)        6 2023-07-31 07:04:07.000000 payme-pkg-2.3/lib/payme_pkg.egg-info/top_level.txt
+-rw-r--r--   0 thenight   (501) staff       (20)      107 2023-07-31 07:04:07.224736 payme-pkg-2.3/setup.cfg
+-rw-r--r--   0 thenight   (501) staff       (20)      538 2023-07-31 07:03:48.000000 payme-pkg-2.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `payme-pkg-2.2/README.md` & `payme-pkg-2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,136 +1,154 @@
 # Payme Uzbekistan Integration Uzcard and Humo
+
 <p align="center">
-    <img style="width: 70%;" src="https://www.gazeta.uz/media/img/2019/07/GDpmEM15631750293941_b.jpg"></img>
+    <img style="width: 60%;" src="https://www.gazeta.uz/media/img/2019/07/GDpmEM15631750293941_b.jpg"></img>
 </p>
 
 Support Group - https://t.me/+Ng1axYLNyBAyYTRi <br/>
 Implementation Sample - https://github.com/Muhammadali-Akbarov/payme-sample
 
 ## Installation
 
+```shell
+pip install payme-pkg
 ```
-$ pip install payme-pkg
-```
+
 ### Test-Credentials
+
 ```
-Card Numer: 8600 4954 7331 6478 Expire Date: 03/99 SMS Code: 666666 
-Card Numer: 8600 0691 9540 6311 Expire Date: 03/99 SMS Code: 666666 
+Card Numer: 8600 4954 7331 6478 Expire Date: 03/99 SMS Code: 666666
+Card Numer: 8600 0691 9540 6311 Expire Date: 03/99 SMS Code: 666666
 ```
 
 ## Documentation
-  * [Merchant API](#merchant-api)
-  * [Generate Pay Link](#generate-pay-link)
-  * Subscribe Cards
-    * [Cards Create](#cards-create)
-    * [Cards Get Verify Code](#cards-get-verify-code)
-    * [Cards Verify](#cards-verify)
-    * [Cards Check](#cards-check)
-    * [Cards Remove](#cards-remove)
-   
-  * Subscribe Receipts
-    * [Receipts Create](#receipts-create)
-    * [Receipts Pay](#receipts-pay)
-    * [Receipts Send](#receipts-send)
-    * [Receipts Cancel](#receipts-cancel)
-    * [Receipts Check](#receipts-check)
-    * [Receipts Get](#receipts-get)
-    * [Receipts Get All ](#receipts-get-all)
+
+- [Merchant API](#merchant-api)
+- [Generate Pay Link](#generate-pay-link)
+
+- Subscribe Cards
+
+  - [Cards Create](#cards-create)
+  - [Cards Get Verify Code](#cards-get-verify-code)
+  - [Cards Verify](#cards-verify)
+  - [Cards Check](#cards-check)
+  - [Cards Remove](#cards-remove)
+
+- Subscribe Receipts
+  - [Receipts Create](#receipts-create)
+  - [Receipts Pay](#receipts-pay)
+  - [Receipts Send](#receipts-send)
+  - [Receipts Cancel](#receipts-cancel)
+  - [Receipts Check](#receipts-check)
+  - [Receipts Get](#receipts-get)
+  - [Receipts Get All ](#receipts-get-all)
 
 # Merchant API
 
 ## Installation to Django
 
 Add `'payme'` in to your settings.
+
 ```python
 INSTALLED_APPS = [
     ...
     'payme',
     ...
 ]
 ```
+
 Add `'payme'` credentials inside to settings.
+
 ```python
 PAYME: dict = {
     'PAYME_ID': 'payme-id',
     'PAYME_KEY': 'payme-key',
     'PAYME_URL': 'payme-checkout-url',
     'PAYME_CALL_BACK_URL': 'your-callback-url', # merchant api callback url
     'PAYME_MIN_AMOUNT': 'payme-min-amount', # integer field
     'PAYME_ACCOUNT': 'order-id',
 }
 
 ORDER_MODEL = 'your_app.models.Your_Order_Model'
 ```
+
 Add a `payme` path to core of urlpatterns:
+
 ```python
 from django.urls import path
 from django.urls import include
 
 urlpatterns = [
     ...
     path("payments/", include("payme.urls"))
     ...
 ]
 ```
+
 Run migrations
+
+```shell
+python manage.py migrate
 ```
-$ python manage.py migrate
-```
-🎉 Congratulations you have been integrated merchant api methods with django, keep reading docs.After successfull migrations check your admin panel and see results what happened.
+
+🎉 Congratulations you have been integrated merchant api methods with django, keep reading docs. After successfull migrations check your admin panel and see results what happened.
 
 ## Generate Pay Link
+
 Example to generate link:
 
-* Input
+- Input
 
 ```python
 from pprint import pprint
 
 from payme.methods.generate_link import GeneratePayLink
 
 pay_link = GeneratePayLink(
   order_id=999,
   amount=9999
 ).generate_link()
 
 pprint(pay_link)
 ```
-* Output
+
+- Output
 
 ```
 Link: https://checkout.paycom.uz/bT01ZTczMGU4ZTBiODUyYTQxN2FhNDljZWI7YWMub3JkZXItaWQ9OTk5O2E9OTk5OTtjPXlvdXItY2FsbGJhY2stdXJs
 ```
+
 ## Cards Create
+
 Example for cards create method for to generate token from card:
 
-* Request
+- Request
 
-```
+```python
 from pprint import pprint
 
 from payme.cards.subscribe_cards import PaymeSubscribeCards
 
-
 client = PaymeSubscribeCards(
     base_url="https://checkout.test.paycom.uz/api/",
     paycom_id="5e730e8e0b852a417aa49ceb"
 )
 
 resp = client.cards_create(
     number="8600069195406311",
     expire="0399",
-    save=True,
+    save=True
 )
 
 pprint(resp)
 ```
-* Response
 
-```
+- Response
+
+```json
 {
   "jsonrpc": "2.0",
   "result": {
     "card": {
       "number": "860006******6311",
       "expire": "03/99",
       "token": "63119784d15d8d8d093b37b8_ADHrAykwnAIc2hm4hPPriktZ8nnuvR96S9Kzmjb3Fcix25IrJmMKrGxP9VUEP9rRDKRhtYjUw0vsXON7PYEyMCHtDKpMuM4krrIk8jdnyK7bXkSBSCyiGs2aahIrep6TSodIAxqutMJ4g3O8FZ8vC1DSMKzOaX0UF8fDKNexXV039Qnj4bNQc6NcpKGJn0wUX8d0RBqkmKid4WyUQnT987ZQDM2mT2IGNZtugvN4tDJTXBVTpqCWkXnZ0YWj64Ye0ztr91Mibtndo0Y1s5nCA6wufUZZugJ6c7rse19XNFSSieFM7AWi9VqybMe4eeWiZEBriAbFhrf8kQvrpBmwUEp05GjvFMgH0ku3vyUtSuJI36exHheXuJK66KstcX1i69EaF3",
@@ -139,17 +157,20 @@
       "type": "22618"
     }
   }
 }
 ```
 
 ## Cards Get Verify Code
+
 Example for cards get verify:
-* Request
-```
+
+- Request
+
+```python
 from pprint import pprint
 
 from payme.cards.subscribe_cards import PaymeSubscribeCards
 
 
 client = PaymeSubscribeCards(
     base_url="https://checkout.test.paycom.uz/api/",
@@ -158,30 +179,35 @@
 
 resp = client.card_get_verify_code(
     token="630e5ffdd15d8d8d093b379b_2fsaoABWafecn20kofV4PFafFZjeGDWS9adM1PmboQaEZbbaxMcnaskctMbU9Iv8qgrOuKGz8SnjvZvYXDK64m1eS9gA5jZ7BBRaQybMXrDPtFPJ1fwek5B1KoIv5cMiCWYXj7ezpYEdJAKTIQw0Np9HsTXjqco4gQG3m8MOfeH9ovkdm66O6yj45oKXRmJyAK5i0SchXNNomACH3Oq80KyoRE1VoBRxvoKyMkOx0xcepXovxK9d3v26a8z7UtyokwY33N8MupviM3A5WHB5Xh35WZJJyFnxTSi1vvnYnG7uVd6Bb1GjV2yAHnimss8aEZGW5V7ZiPrhf8r6WJAeHciYDGK3msRKZJBQTfjgOdE9tGrEnMezVkxr1JXX0xSn5qqec2"
 )
 
 pprint(resp)
 ```
-* Response
-```
+
+- Response
+
+```json
 {
   "jsonrpc": "2.0",
   "result": {
     "sent": true,
     "phone": "99890*****66",
     "wait": 60000
   }
 }
 ```
 
 ## Cards Verify
+
 Example for cards verify method:
-* Request
-```
+
+- Request
+
+```python
 from pprint import pprint
 
 from payme.cards.subscribe_cards import PaymeSubscribeCards
 
 
 client = PaymeSubscribeCards(
     base_url="https://checkout.test.paycom.uz/api/",
@@ -191,16 +217,18 @@
 resp = client.cards_verify(
     verify_code="666666",
     token="630e691fd15d8d8d093b379c_70mKyzqS8d1wTWzovIGjt9dKmjpn1KI8Y9XakPrfpbUASTBaZYbC1DjDcjYRmuNJep9gZrTRtHyEGBQYmBaPufuozF51bv4qEPsQnodq1VcD7tYyREwUXjMXXZUeu7Ek0REQCekCvVHX6rtNBpb4vtViJoNVjp94XpTqu0Bn3yYYb0CHu951wFydzRsieGxjGNrvx1oKyBcq0CdOUwoffRIt2VPvx5R2aVmc6ahwyhn387FEEcpO1PnjIJkWKTBWdI35ZPQnb1u1oss5aPg06E279THXRkoTThixbeqiD2JkWSXweNVGGDhTS30V4j61G3NWEPO2H3k4uFmCjjIQSzx4TxKzUgHg1i2q953PRUGjT4JZBRHMDxaN5tWuctEMNmY06p"
 )
 
 pprint(resp)
 ```
-* Response
-```
+
+- Response
+
+```json
 {
   "jsonrpc": "2.0",
   "result": {
     "card": {
       "number": "860006******6311",
       "expire": "03/99",
       "token": "63118a5dd15d8d8d093b37b7_X2j34OIJPnROfsgzYZCZ0w7OcC50zzwiowTsotEVO1uUbxkzaDrvdOno6jicQTrcRmxvibxrye4vUS3AynTNPaPCTGpfk3RCKmT9NaOAyyTmctAjWsjwvqGR5XUzAP1Xcx12GkhuQi6VJ4BeaIXOokSRu06rRjaivmJQ8HTiJiR9b3OmZtrhkIRNcNXnnp9zYm1mFP4BuqGpS8BMnY0ASIE6ffxWykjgBcDTAfWBFt4mg7O9Dsvx0aj3IB8z3RIbZYtDZJnUVhCZrwW7ONVI9uEAdxNthorjO6PbV7TQ8XCjrztgGf6uCtOwwxasiIUVZN6tCVDk8A8NvVSUzUHXQHVkaPn5heJNa3K4WsffIckq7SwMbiw3UbawipeZKyD3iwk1Km",
@@ -209,17 +237,20 @@
       "type": "22618"
     }
   }
 }
 ```
 
 ## Cards Check
+
 Example for cards check:
-* Request
-```
+
+- Request
+
+```python
 from pprint import pprint
 
 from payme.cards.subscribe_cards import PaymeSubscribeCards
 
 
 client = PaymeSubscribeCards(
     base_url="https://checkout.test.paycom.uz/api/",
@@ -228,34 +259,40 @@
 
 resp = client.cards_check(
     token="630e691fd15d8d8d093b379c_70mKyzqS8d1wTWzovIGjt9dKmjpn1KI8Y9XakPrfpbUASTBaZYbC1DjDcjYRmuNJep9gZrTRtHyEGBQYmBaPufuozF51bv4qEPsQnodq1VcD7tYyREwUXjMXXZUeu7Ek0REQCekCvVHX6rtNBpb4vtViJoNVjp94XpTqu0Bn3yYYb0CHu951wFydzRsieGxjGNrvx1oKyBcq0CdOUwoffRIt2VPvx5R2aVmc6ahwyhn387FEEcpO1PnjIJkWKTBWdI35ZPQnb1u1oss5aPg06E279THXRkoTThixbeqiD2JkWSXweNVGGDhTS30V4j61G3NWEPO2H3k4uFmCjjIQSzx4TxKzUgHg1i2q953PRUGjT4JZBRHMDxaN5tWuctEMNmY06p"
 )
 
 pprint(resp)
 ```
-* Response
-```
+
+- Response
+
+```json
 {
   "jsonrpc": "2.0",
   "result": {
     "card": {
       "number": "860006******6311",
       "expire": "03/99",
       "token": "63119b36d15d8d8d093b37c1_IJtHxZ46h5viyo8RIJCmQyE8qBw6PUWUdFKTMCVWrPoMMi4kJYsKyVdjQrIx6a12jDfEPVhhEqWm94FYvYh7IEjIs4xn0n3mM8Quw5dhd6ZT0dOK6u1spqWRMIDBpDMhHj2Ga8zZMAfeoiDAcrWScXS1AP2tkQHcJ40rBzHGHS6DoVeIheF70c0wO1kVQG0G5hDWguSGf2ZRFcBtpabv5BQkqSchxWKdCSVPIGiS6X7eF8YStdz1aGPzFyjDbaKT0vXNUMbQ7gaKh4PeQbruVVwFDfeIWqGeNmgCCPU4X0wCHFjTt8K61e9VOauNeU81ckoKHD8XGzCwGFJHrC4sHvNv4no3RifWhHCQF9GmFKf8cP2qh4pqTKwu3gOITaX5Ss71tC",
       "recurrent": true,
       "verify": true,
       "type": "22618"
     }
   }
 }
 ```
+
 ## Cards Remove
+
 Example for cards create method for to generate token from card:
-* Request
-```
+
+- Request
+
+```python
 from pprint import pprint
 
 from payme.cards.subscribe_cards import PaymeSubscribeCards
 
 
 client = PaymeSubscribeCards(
     base_url="https://checkout.test.paycom.uz/api/",
@@ -264,27 +301,33 @@
 
 resp = client.cards_remove(
     token="630e691fd15d8d8d093b379c_70mKyzqS8d1wTWzovIGjt9dKmjpn1KI8Y9XakPrfpbUASTBaZYbC1DjDcjYRmuNJep9gZrTRtHyEGBQYmBaPufuozF51bv4qEPsQnodq1VcD7tYyREwUXjMXXZUeu7Ek0REQCekCvVHX6rtNBpb4vtViJoNVjp94XpTqu0Bn3yYYb0CHu951wFydzRsieGxjGNrvx1oKyBcq0CdOUwoffRIt2VPvx5R2aVmc6ahwyhn387FEEcpO1PnjIJkWKTBWdI35ZPQnb1u1oss5aPg06E279THXRkoTThixbeqiD2JkWSXweNVGGDhTS30V4j61G3NWEPO2H3k4uFmCjjIQSzx4TxKzUgHg1i2q953PRUGjT4JZBRHMDxaN5tWuctEMNmY06p"
 )
 
 pprint(resp)
 ```
-* Response
-```
+
+- Response
+
+```json
 {
   "jsonrpc": "2.0",
   "result": {
     "success": true
   }
 }
 ```
+
 ## Receipts Create
+
 Example for receipts create method:
-* Request
-```
+
+- Request
+
+```python
 from pprint import pprint
 
 from payme.receipts.subscribe_receipts import PaymeSubscribeReceipts
 
 
 rclient = PaymeSubscribeReceipts(
     base_url="https://checkout.test.paycom.uz/api/",
@@ -295,16 +338,18 @@
 resp = rclient.receipts_create(
     amount=10000,
     order_id="1"
 )
 
 pprint(resp)
 ```
-* Response
-```
+
+- Response
+
+```json
 {
   "jsonrpc": "2.0",
   "result": {
     "receipt": {
       "_id": "63119becc4420cbf2712a24c",
       "create_time": 1662098412270,
       "pay_time": 0,
@@ -349,18 +394,22 @@
         "owner": "5e730e8e0b852a417aa49ceb"
       },
       "processing_id": null
     }
   }
 }
 ```
+
 ## Receipts Pay
+
 Example for receipts pay method:
-* Request
-```
+
+- Request
+
+```python
 from pprint import pprint
 
 from payme.receipts.subscribe_receipts import PaymeSubscribeReceipts
 
 
 rclient = PaymeSubscribeReceipts(
     base_url="https://checkout.test.paycom.uz/api/",
@@ -372,16 +421,18 @@
     invoice_id="631186b6c4420cbf2712a243",
     token="63118a5dd15d8d8d093b37b7_X2j34OIJPnROfsgzYZCZ0w7OcC50zzwiowTsotEVO1uUbxkzaDrvdOno6jicQTrcRmxvibxrye4vUS3AynTNPaPCTGpfk3RCKmT9NaOAyyTmctAjWsjwvqGR5XUzAP1Xcx12GkhuQi6VJ4BeaIXOokSRu06rRjaivmJQ8HTiJiR9b3OmZtrhkIRNcNXnnp9zYm1mFP4BuqGpS8BMnY0ASIE6ffxWykjgBcDTAfWBFt4mg7O9Dsvx0aj3IB8z3RIbZYtDZJnUVhCZrwW7ONVI9uEAdxNthorjO6PbV7TQ8XCjrztgGf6uCtOwwxasiIUVZN6tCVDk8A8NvVSUzUHXQHVkaPn5heJNa3K4WsffIckq7SwMbiw3UbawipeZKyD3iwk1Km",
     phone="998901304527"
 )
 
 pprint(resp)
 ```
-* Response
-```
+
+- Response
+
+```json
 {
   "jsonrpc": "2.0",
   "id": 123,
   "result": {
     "receipt": {
       "_id": "63119becc4420cbf2712a24c",
       "create_time": 1662098438706,
@@ -430,18 +481,22 @@
         "owner": "5e730e8e0b852a417aa49ceb"
       },
       "processing_id": 0
     }
   }
 }
 ```
+
 ## Receipts Send
+
 Example for receipts send method:
-* Request
-```
+
+- Request
+
+```python
 from pprint import pprint
 
 from payme.receipts.subscribe_receipts import PaymeSubscribeReceipts
 
 
 rclient = PaymeSubscribeReceipts(
     base_url="https://checkout.test.paycom.uz/api/",
@@ -452,28 +507,34 @@
 resp = rclient.receipts_send(
     invoice_id="631186b6c4420cbf2712a243",
     phone="998901304527"
 )
 
 pprint(resp)
 ```
-* Response
-```
+
+- Response
+
+```json
 {
   "jsonrpc": "2.0",
   "id": 123,
   "result": {
     "success": true
   }
 }
 ```
+
 ## Receipts Cancel
+
 Example for receipts cancel method:
-* Request
-```
+
+- Request
+
+```python
 from pprint import pprint
 
 from payme.receipts.subscribe_receipts import PaymeSubscribeReceipts
 
 
 rclient = PaymeSubscribeReceipts(
     base_url="https://checkout.test.paycom.uz/api/",
@@ -483,16 +544,18 @@
 
 resp = rclient.receipts_cancel(
     invoice_id="63119303c4420cbf2712a245"
 )
 
 pprint(resp)
 ```
-* Response
-```
+
+- Response
+
+```json
 {
   "jsonrpc": "2.0",
   "id": 123,
   "result": {
     "receipt": {
       "_id": "63119becc4420cbf2712a24c",
       "create_time": 1662098438706,
@@ -542,18 +605,22 @@
         "source_cancel": "subscribe"
       },
       "processing_id": null
     }
   }
 }
 ```
+
 ## Receipts Check
+
 Example for receipts check method:
-* Request
-```
+
+- Request
+
+```python
 from pprint import pprint
 
 from payme.receipts.subscribe_receipts import PaymeSubscribeReceipts
 
 
 rclient = PaymeSubscribeReceipts(
     base_url="https://checkout.test.paycom.uz/api/",
@@ -563,28 +630,34 @@
 
 resp = rclient.receipts_check(
     invoice_id="63119303c4420cbf2712a245"
 )
 
 pprint(resp)
 ```
-* Response
-```
+
+- Response
+
+```json
 {
   "jsonrpc": "2.0",
   "id": 123,
   "result": {
     "state": 0
   }
 }
 ```
+
 ## Receipts Get
+
 Example for receipts get method:
-* Request
-```
+
+- Request
+
+```python
 from pprint import pprint
 
 from payme.receipts.subscribe_receipts import PaymeSubscribeReceipts
 
 
 rclient = PaymeSubscribeReceipts(
     base_url="https://checkout.test.paycom.uz/api/",
@@ -594,16 +667,18 @@
 
 resp = rclient.reciepts_get(
     invoice_id="6311946bc4420cbf2712a247"
 )
 
 pprint(resp)
 ```
-* Response
-```
+
+- Response
+
+```json
 {
   "jsonrpc": "2.0",
   "id": 123,
   "result": {
     "receipt": {
       "_id": "6311946bc4420cbf2712a247",
       "create_time": 1662096491076,
@@ -649,18 +724,22 @@
         "owner": "5e730e8e0b852a417aa49ceb"
       },
       "processing_id": null
     }
   }
 }
 ```
+
 ## Receipts Get All
+
 Example for receipts get all method:
-* Request
-```
+
+- Request
+
+```python
 from pprint import pprint
 
 from payme.receipts.subscribe_receipts import PaymeSubscribeReceipts
 
 
 rclient = PaymeSubscribeReceipts(
     base_url="https://checkout.test.paycom.uz/api/",
@@ -673,16 +752,18 @@
     _from=1636398000000,
     to=1636398000000,
     offset=0
 )
 
 pprint(resp)
 ```
-* Response
-```
+
+- Response
+
+```json
 {
   "jsonrpc": "2.0",
   "id": 123,
   "result": [
     {
       "_id": "6311946bc4420cbf2712a247",
       "create_time": 1662096491076,
@@ -786,8 +867,8 @@
         "owner": "5e730e8e0b852a417aa49ceb",
         "source_cancel": "subscribe"
       },
       "processing_id": null
     }
   ]
 }
-
+```
```

### Comparing `payme-pkg-2.2/setup.py` & `payme-pkg-2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='payme-pkg',
-    version='2.2',
+    version='2.3',
     license='MIT',
     author="Muhammadali Akbarov",
     author_email='muhammadali17abc@gmail.com',
     packages=find_packages('lib'),
     package_dir={'': 'lib'},
     url='https://github.com/Muhammadali-Akbarov/payme-pkg',
     keywords='paymeuz paycomuz payme-merchant merchant-api subscribe-api payme-pkg payme-api',
```

### Comparing `payme-pkg-2.2/lib/payme_pkg.egg-info/SOURCES.txt` & `payme-pkg-2.3/lib/payme_pkg.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.md
 setup.cfg
 setup.py
 lib/payme/__init__.py
 lib/payme/admin.py
 lib/payme/apps.py
 lib/payme/models.py
@@ -16,22 +17,24 @@
 lib/payme/errors/exceptions.py
 lib/payme/methods/__init__.py
 lib/payme/methods/cancel_transaction.py
 lib/payme/methods/check_perform_transaction.py
 lib/payme/methods/check_transaction.py
 lib/payme/methods/create_transaction.py
 lib/payme/methods/generate_link.py
+lib/payme/methods/get_statement.py
 lib/payme/methods/perform_transaction.py
 lib/payme/migrations/0001_initial.py
 lib/payme/migrations/__init__.py
 lib/payme/receipts/__init__.py
 lib/payme/receipts/subscribe_receipts.py
 lib/payme/utils/__init__.py
 lib/payme/utils/get_params.py
 lib/payme/utils/logging.py
+lib/payme/utils/make_aware_datetime.py
 lib/payme/utils/support.py
 lib/payme/utils/to_json.py
 lib/payme_pkg.egg-info/PKG-INFO
 lib/payme_pkg.egg-info/SOURCES.txt
 lib/payme_pkg.egg-info/dependency_links.txt
 lib/payme_pkg.egg-info/requires.txt
 lib/payme_pkg.egg-info/top_level.txt
```

### Comparing `payme-pkg-2.2/lib/payme/receipts/subscribe_receipts.py` & `payme-pkg-2.3/lib/payme/receipts/subscribe_receipts.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.2/lib/payme/migrations/0001_initial.py` & `payme-pkg-2.3/lib/payme/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.2/lib/payme/methods/check_perform_transaction.py` & `payme-pkg-2.3/lib/payme/methods/check_perform_transaction.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.2/lib/payme/methods/cancel_transaction.py` & `payme-pkg-2.3/lib/payme/methods/cancel_transaction.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.2/lib/payme/methods/create_transaction.py` & `payme-pkg-2.3/lib/payme/methods/create_transaction.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.2/lib/payme/methods/perform_transaction.py` & `payme-pkg-2.3/lib/payme/methods/perform_transaction.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.2/lib/payme/methods/generate_link.py` & `payme-pkg-2.3/lib/payme/methods/generate_link.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.2/lib/payme/methods/check_transaction.py` & `payme-pkg-2.3/lib/payme/methods/check_transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from django.db import DatabaseError
 
 from payme.utils.logging import logger
 from payme.models import MerchatTransactionsModel
 from payme.serializers import MerchatTransactionsModelSerializer as MTMS
```

### Comparing `payme-pkg-2.2/lib/payme/models.py` & `payme-pkg-2.3/lib/payme/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,24 +22,25 @@
     created_at_ms = models.CharField(max_length=255, null=True, blank=True)
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
 
     def __str__(self):
         return str(self._id)
 
+
 try:
     CUSTOM_ORDER = import_string(settings.ORDER_MODEL)
     if 'amount' in CUSTOM_ORDER.__doc__:
         Order = CUSTOM_ORDER
     else:
         raise ImportError("amount field is not defined in your custom order model")
 
 except (ImportError, AttributeError):
     CUSTOM_ORDER = None
-    logger.warning("Your have no payme custom order model")
+    logger.warning("You have no payme custom order model")
 
     class Order(models.Model):
         """
         Order class \
             That's used for managing order process
         """
         amount = models.IntegerField(null=True, blank=True)
```

### Comparing `payme-pkg-2.2/lib/payme/decorators/decorators.py` & `payme-pkg-2.3/lib/payme/decorators/decorators.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.2/lib/payme/cards/subscribe_cards.py` & `payme-pkg-2.3/lib/payme/cards/subscribe_cards.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.2/lib/payme/serializers.py` & `payme-pkg-2.3/lib/payme/serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,22 @@
 
 
 class MerchatTransactionsModelSerializer(serializers.ModelSerializer):
     """
     MerchatTransactionsModelSerializer class \
         That's used to serialize merchat transactions data.
     """
+    start_date = serializers.IntegerField(allow_null=True)
+    end_date = serializers.IntegerField(allow_null=True)
+
     class Meta:
         # pylint: disable=missing-class-docstring
         model: MerchatTransactionsModel = MerchatTransactionsModel
         fields: str = "__all__"
+        extra_fields = ['start_date', 'end_date']
 
     def validate(self, attrs) -> dict:
         """
         Validate the data given to the MerchatTransactionsModel.
         """
         if attrs.get("order_id") is not None:
             try:
```

### Comparing `payme-pkg-2.2/lib/payme/utils/get_params.py` & `payme-pkg-2.3/lib/payme/utils/get_params.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
     clean_params: dict = {}
     clean_params["_id"] = params.get("id")
     clean_params["time"] = params.get("time")
     clean_params["amount"] = params.get("amount")
     clean_params["reason"] = params.get("reason")
 
-    if params.get("reason") is not None:
-        clean_params["reason"] = params.get("reason")
+    # get statement method params
+    clean_params["start_date"] = params.get("from")
+    clean_params["end_date"] = params.get("to")
 
     if account is not None:
         account_name: str = settings.PAYME.get("PAYME_ACCOUNT")
         clean_params["order_id"] = account[account_name]
 
     return clean_params
```

### Comparing `payme-pkg-2.2/lib/payme/errors/exceptions.py` & `payme-pkg-2.3/lib/payme/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `payme-pkg-2.2/lib/payme/views.py` & `payme-pkg-2.3/lib/payme/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,32 +14,34 @@
 from payme.errors.exceptions import PerformTransactionDoesNotExist
 
 from payme.methods.check_transaction import CheckTransaction
 from payme.methods.cancel_transaction import CancelTransaction
 from payme.methods.create_transaction import CreateTransaction
 from payme.methods.perform_transaction import PerformTransaction
 from payme.methods.check_perform_transaction import CheckPerformTransaction
+from payme.methods.get_statement import GetStatement
 
 
 class MerchantAPIView(APIView):
     """
     MerchantAPIView class provides payme call back functionality.
     """
     permission_classes = ()
     authentication_classes = ()
 
     def post(self, request) -> Response:
         """
         Payme sends post request to our call back url.
         That methods are includes 5 methods
-            - CheckTransaction
+            - CheckPerformTransaction
             - CreateTransaction
-            - CancelTransaction
             - PerformTransaction
-            - CheckPerformTransaction
+            - CancelTransaction
+            - CheckTransaction
+            - GetStatement
         """
         password = request.META.get('HTTP_AUTHORIZATION')
         if self.authorize(password):
             incoming_data: dict = request.data
             incoming_method: str = incoming_data.get("method")
 
             logger.info("Call back data is incoming %s", incoming_data)
@@ -63,19 +65,20 @@
     @staticmethod
     def get_paycom_method_by_name(incoming_method: str) -> object:
         """
         Use this static method to get the paycom method by name.
         :param incoming_method: string -> incoming method name
         """
         available_methods: dict = {
-            "CheckTransaction": CheckTransaction,
+            "CheckPerformTransaction": CheckPerformTransaction,
             "CreateTransaction": CreateTransaction,
-            "CancelTransaction": CancelTransaction,
             "PerformTransaction": PerformTransaction,
-            "CheckPerformTransaction": CheckPerformTransaction
+            "CancelTransaction": CancelTransaction,
+            "CheckTransaction": CheckTransaction,
+            "GetStatement": GetStatement
         }
 
         try:
             merchant_method = available_methods[incoming_method]
         except Exception as error:
             error_message = "Unavailable method: %s", incoming_method
             logger.error(error_message)
```

