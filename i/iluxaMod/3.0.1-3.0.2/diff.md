# Comparing `tmp/iluxaMod-3.0.1.tar.gz` & `tmp/iluxaMod-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iluxaMod-3.0.1.tar", last modified: Mon Jul 31 19:19:35 2023, max compression
+gzip compressed data, was "iluxaMod-3.0.2.tar", last modified: Mon Jul 31 19:34:33 2023, max compression
```

## Comparing `iluxaMod-3.0.1.tar` & `iluxaMod-3.0.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 19:19:35.221630 iluxaMod-3.0.1/
--rw-rw-rw-   0        0        0     5518 2023-07-31 19:19:35.221630 iluxaMod-3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4595 2023-07-31 16:36:57.000000 iluxaMod-3.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 19:19:35.212713 iluxaMod-3.0.1/iluxaMod/
--rw-rw-rw-   0        0        0      357 2023-07-31 19:19:31.000000 iluxaMod-3.0.1/iluxaMod/__init__.py
--rw-rw-rw-   0        0        0      817 2023-07-31 19:12:39.000000 iluxaMod-3.0.1/iluxaMod/arduino.py
--rw-rw-rw-   0        0        0     3152 2023-07-31 19:19:31.000000 iluxaMod-3.0.1/iluxaMod/automation.py
--rw-rw-rw-   0        0        0      322 2023-07-31 19:12:39.000000 iluxaMod-3.0.1/iluxaMod/barcode.py
--rw-rw-rw-   0        0        0     3239 2023-07-31 19:19:31.000000 iluxaMod-3.0.1/iluxaMod/convertors.py
--rw-rw-rw-   0        0        0      417 2023-07-31 19:12:39.000000 iluxaMod-3.0.1/iluxaMod/distance.py
--rw-rw-rw-   0        0        0      511 2023-07-31 19:19:31.000000 iluxaMod-3.0.1/iluxaMod/keygen.py
--rw-rw-rw-   0        0        0      465 2023-07-31 19:19:31.000000 iluxaMod-3.0.1/iluxaMod/pickle.py
--rw-rw-rw-   0        0        0    10861 2023-07-31 17:09:30.000000 iluxaMod-3.0.1/iluxaMod/postgreSQL.py
--rw-rw-rw-   0        0        0      455 2023-07-31 19:12:39.000000 iluxaMod-3.0.1/iluxaMod/qr.py
--rw-rw-rw-   0        0        0      462 2023-07-31 19:19:31.000000 iluxaMod-3.0.1/iluxaMod/termux.py
--rw-rw-rw-   0        0        0      864 2023-07-31 19:12:39.000000 iluxaMod-3.0.1/iluxaMod/tgbot.py
--rw-rw-rw-   0        0        0      174 2023-07-31 19:19:31.000000 iluxaMod-3.0.1/iluxaMod/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-31 19:19:35.220131 iluxaMod-3.0.1/iluxaMod.egg-info/
--rw-rw-rw-   0        0        0     5518 2023-07-31 19:19:35.000000 iluxaMod-3.0.1/iluxaMod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      436 2023-07-31 19:19:35.000000 iluxaMod-3.0.1/iluxaMod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 19:19:35.000000 iluxaMod-3.0.1/iluxaMod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-07-31 19:19:35.000000 iluxaMod-3.0.1/iluxaMod.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-31 19:19:35.000000 iluxaMod-3.0.1/iluxaMod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 19:19:35.222654 iluxaMod-3.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1789 2023-07-31 19:19:31.000000 iluxaMod-3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 19:34:33.415479 iluxaMod-3.0.2/
+-rw-rw-rw-   0        0        0     5518 2023-07-31 19:34:33.415479 iluxaMod-3.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4595 2023-07-31 16:36:57.000000 iluxaMod-3.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 19:34:33.407031 iluxaMod-3.0.2/iluxaMod/
+-rw-rw-rw-   0        0        0      380 2023-07-31 19:27:44.000000 iluxaMod-3.0.2/iluxaMod/__init__.py
+-rw-rw-rw-   0        0        0      817 2023-07-31 19:12:39.000000 iluxaMod-3.0.2/iluxaMod/arduino.py
+-rw-rw-rw-   0        0        0     3152 2023-07-31 19:19:31.000000 iluxaMod-3.0.2/iluxaMod/automation.py
+-rw-rw-rw-   0        0        0      322 2023-07-31 19:12:39.000000 iluxaMod-3.0.2/iluxaMod/barcode.py
+-rw-rw-rw-   0        0        0     3239 2023-07-31 19:19:31.000000 iluxaMod-3.0.2/iluxaMod/convertors.py
+-rw-rw-rw-   0        0        0      417 2023-07-31 19:12:39.000000 iluxaMod-3.0.2/iluxaMod/distance.py
+-rw-rw-rw-   0        0        0      511 2023-07-31 19:19:31.000000 iluxaMod-3.0.2/iluxaMod/keygen.py
+-rw-rw-rw-   0        0        0      358 2023-07-31 19:33:57.000000 iluxaMod-3.0.2/iluxaMod/mechanics.py
+-rw-rw-rw-   0        0        0      465 2023-07-31 19:19:31.000000 iluxaMod-3.0.2/iluxaMod/pickle.py
+-rw-rw-rw-   0        0        0    10861 2023-07-31 17:09:30.000000 iluxaMod-3.0.2/iluxaMod/postgreSQL.py
+-rw-rw-rw-   0        0        0      455 2023-07-31 19:12:39.000000 iluxaMod-3.0.2/iluxaMod/qr.py
+-rw-rw-rw-   0        0        0      462 2023-07-31 19:19:31.000000 iluxaMod-3.0.2/iluxaMod/termux.py
+-rw-rw-rw-   0        0        0      864 2023-07-31 19:12:39.000000 iluxaMod-3.0.2/iluxaMod/tgbot.py
+-rw-rw-rw-   0        0        0      176 2023-07-31 19:27:44.000000 iluxaMod-3.0.2/iluxaMod/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-31 19:34:33.413463 iluxaMod-3.0.2/iluxaMod.egg-info/
+-rw-rw-rw-   0        0        0     5518 2023-07-31 19:34:33.000000 iluxaMod-3.0.2/iluxaMod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      458 2023-07-31 19:34:33.000000 iluxaMod-3.0.2/iluxaMod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 19:34:33.000000 iluxaMod-3.0.2/iluxaMod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-07-31 19:34:33.000000 iluxaMod-3.0.2/iluxaMod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 19:34:33.000000 iluxaMod-3.0.2/iluxaMod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 19:34:33.416531 iluxaMod-3.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1789 2023-07-31 19:33:57.000000 iluxaMod-3.0.2/setup.py
```

### Comparing `iluxaMod-3.0.1/PKG-INFO` & `iluxaMod-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iluxaMod
-Version: 3.0.1
+Version: 3.0.2
 Summary: Module for simplified work with libraries: TG, PostgreSQL, locations and more...
 Home-page: https://sbdt.pro
 Author: Illya Lazarev
 Author-email: lazarevillya031@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `iluxaMod-3.0.1/README.md` & `iluxaMod-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `iluxaMod-3.0.1/iluxaMod/arduino.py` & `iluxaMod-3.0.2/iluxaMod/arduino.py`

 * *Files identical despite different names*

### Comparing `iluxaMod-3.0.1/iluxaMod/automation.py` & `iluxaMod-3.0.2/iluxaMod/automation.py`

 * *Files identical despite different names*

### Comparing `iluxaMod-3.0.1/iluxaMod/convertors.py` & `iluxaMod-3.0.2/iluxaMod/convertors.py`

 * *Files identical despite different names*

### Comparing `iluxaMod-3.0.1/iluxaMod/postgreSQL.py` & `iluxaMod-3.0.2/iluxaMod/postgreSQL.py`

 * *Files identical despite different names*

### Comparing `iluxaMod-3.0.1/iluxaMod/tgbot.py` & `iluxaMod-3.0.2/iluxaMod/tgbot.py`

 * *Files identical despite different names*

### Comparing `iluxaMod-3.0.1/iluxaMod.egg-info/PKG-INFO` & `iluxaMod-3.0.2/iluxaMod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iluxaMod
-Version: 3.0.1
+Version: 3.0.2
 Summary: Module for simplified work with libraries: TG, PostgreSQL, locations and more...
 Home-page: https://sbdt.pro
 Author: Illya Lazarev
 Author-email: lazarevillya031@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `iluxaMod-3.0.1/setup.py` & `iluxaMod-3.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def readme() -> str:
     with open('README.md', 'r', encoding='utf-8') as f:
         return str(f.read())
 
 
 setup(
     name='iluxaMod',
-    version='3.0.1',  # Версия вашего пакета
+    version='3.0.2',  # Версия вашего пакета
     packages=['iluxaMod'],  # Автоматически найдет все пакеты в корневой директории
     install_requires=[  # Зависимости вашего пакета
         'geopy',
         'psycopg2-binary',
         'pyTelegramBotAPI',
         'requests',
         'pyfirmata',
```

