# Comparing `tmp/AshCrypt-3.0.5.tar.gz` & `tmp/AshCrypt-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AshCrypt-3.0.5.tar", last modified: Wed Jul 26 13:11:04 2023, max compression
+gzip compressed data, was "dist/AshCrypt-3.0.6.tar", last modified: Mon Jul 31 17:53:15 2023, max compression
```

## Comparing `AshCrypt-3.0.5.tar` & `AshCrypt-3.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:11:04.000000 AshCrypt-3.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:11:04.000000 AshCrypt-3.0.5/AshCrypt/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/AshCrypt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/AshCrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/AshCrypt/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/AshCrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/AshCrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/AshCrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    39164 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/AshCrypt/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/AshCrypt/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/AshCrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:11:04.000000 AshCrypt-3.0.5/AshCrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/AshCrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/AshCrypt/unittests/unittest_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:11:04.000000 AshCrypt-3.0.5/AshCrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-26 13:11:04.000000 AshCrypt-3.0.5/AshCrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-26 13:11:04.000000 AshCrypt-3.0.5/AshCrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:11:04.000000 AshCrypt-3.0.5/AshCrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 13:11:04.000000 AshCrypt-3.0.5/AshCrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 13:11:04.000000 AshCrypt-3.0.5/AshCrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-26 13:11:04.000000 AshCrypt-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20174 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 13:11:04.000000 AshCrypt-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-26 13:10:52.000000 AshCrypt-3.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:53:15.000000 AshCrypt-3.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:53:15.000000 AshCrypt-3.0.6/AshCrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/AshCrypt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/AshCrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/AshCrypt/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/AshCrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/AshCrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/AshCrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39164 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/AshCrypt/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/AshCrypt/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/AshCrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:53:15.000000 AshCrypt-3.0.6/AshCrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/AshCrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/AshCrypt/unittests/unittest_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:53:15.000000 AshCrypt-3.0.6/AshCrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-31 17:53:15.000000 AshCrypt-3.0.6/AshCrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-31 17:53:15.000000 AshCrypt-3.0.6/AshCrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:53:15.000000 AshCrypt-3.0.6/AshCrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-31 17:53:15.000000 AshCrypt-3.0.6/AshCrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 17:53:15.000000 AshCrypt-3.0.6/AshCrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-31 17:53:15.000000 AshCrypt-3.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20172 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 17:53:15.000000 AshCrypt-3.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/setup.py
```

### Comparing `AshCrypt-3.0.5/AshCrypt/clicrypt.py` & `AshCrypt-3.0.6/AshCrypt/clicrypt.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from AshCrypt import filecrypt as af
 from AshCrypt import textcrypt as at
+from typing import Optional
 import os.path
 import sys
 
 
 print('Welcome to the CLI')
 
 commands = 'Commands : \n' \
@@ -13,15 +14,20 @@
            '\td : for decryption\n' \
            '\tef : to encrypt a file\n' \
            '\tdf : to decrypt a file\n'
 
 global key
 
 
-def input_selection(q=None, c=None, e=None, d=None, ef=None, df=None):
+def input_selection(q=Optional[int],
+                    c=Optional[int],
+                    e=Optional[int],
+                    d=Optional[int],
+                    ef=Optional[int],
+                    df=Optional[int]):
     global encflag, decFlag, file_decFlag, file_encFlag
     if q == 1:
         sys.exit()
     if c == 1:
         print(commands)
     if e == 1:
         file_decFlag = False
```

### Comparing `AshCrypt-3.0.5/AshCrypt/crypt.py` & `AshCrypt-3.0.6/AshCrypt/crypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.5/AshCrypt/database.py` & `AshCrypt-3.0.6/AshCrypt/database.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.5/AshCrypt/filecrypt.py` & `AshCrypt-3.0.6/AshCrypt/filecrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.5/AshCrypt/gui.py` & `AshCrypt-3.0.6/AshCrypt/gui.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.5/AshCrypt/textcrypt.py` & `AshCrypt-3.0.6/AshCrypt/textcrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.5/AshCrypt/unittests/unittest_crypt.py` & `AshCrypt-3.0.6/AshCrypt/unittests/unittest_crypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.5/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-3.0.6/AshCrypt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 3.0.5
+Version: 3.0.6
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `AshCrypt-3.0.5/PKG-INFO` & `AshCrypt-3.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 3.0.5
+Version: 3.0.6
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `AshCrypt-3.0.5/README.md` & `AshCrypt-3.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 <br>View [Features](https://github.com/AshGw/AES-256#features) Header for more details.
 
 
 
 
 
 ### For Developers ###
-The project uses `crypt` module to ensure secure data encryption and decryption for files and texts while keeping it very easy and simple to use .
+The project uses `crypt` module to ensure secure data encryption and decryption for files and text while keeping it very easy and simple to use .
 view the headers for [filecrypt](https://github.com/AshGw/AES-256#filecrypt) and [textcrypt](https://github.com/AshGw/AES-256#textcrypt) to learn more.
 
 
 It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
 safe and simple manner.
 
 <br>The module has a simple straight forward approach for dealing with sqlite3 databases, even if you're not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check [database](https://github.com/AshGw/AES-256#database-1) header to learn more.
@@ -325,15 +325,15 @@
 ```python
 [{'query 0': ('FAILURE', 'no such table: DoesntExist')}]
 ```
 That's it so simple !
 
 
 ## GUI ##
-The GUI as mentioned above is a fully functional application , you can use it to encrypt files , texts , keep track of files by storing them on demand to a main database , also on demand it can keep track of the keys used for cryptographic operations.
+The GUI as mentioned above is a fully functional application , you can use it to encrypt files , text , keep track of files by storing them on demand to a main database , also on demand it can keep track of the keys used for cryptographic operations.
 ### Usage ###
 1) Set the main key up. If you don't have one , press on the button `generate` to generate a secure safe key ready for use. Then insert it in the `MAINKEY` entry
 2) Now you're able to encrypt files or text (text is limited to 200 characters max)
 ####  Text : 
 - You can insert some text in the entry right below the `TEXT ENCRYPTION` label.<br>The given text will be encrypted and you can choose if you want to have that text displayed as a qr code, a qr image will pop on the screen and you'll be able to scan it using your phone.
 - Insert some encrypted text below the `TEXT DECRYPTION` label.<br>The given text will be decrypted and you'd have the option to display the "plaintext" as a qr code to be scanned by other devices.
 <br>If the text cannot be decrypted it will display itself , so you might as well use this to display the key you're using as a qr code
```

### Comparing `AshCrypt-3.0.5/setup.py` & `AshCrypt-3.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('AshCrypt/README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='3.0.5',
+    version='3.0.6',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along"
                 " with a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

