# Comparing `tmp/otgCrypto-0.0.8.tar.gz` & `tmp/otgCrypto-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otgCrypto-0.0.8.tar", last modified: Wed Jul 26 13:18:01 2023, max compression
+gzip compressed data, was "otgCrypto-0.0.9.tar", last modified: Wed Jul 26 17:47:55 2023, max compression
```

## Comparing `otgCrypto-0.0.8.tar` & `otgCrypto-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 13:18:01.688196 otgCrypto-0.0.8/
--rw-rw-rw-   0        0        0    35821 2023-07-26 09:00:53.000000 otgCrypto-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0     3443 2023-07-26 13:18:01.682160 otgCrypto-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2781 2023-07-26 13:17:44.000000 otgCrypto-0.0.8/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 13:18:01.680161 otgCrypto-0.0.8/otgCrypto.egg-info/
--rw-rw-rw-   0        0        0     3443 2023-07-26 13:18:01.000000 otgCrypto-0.0.8/otgCrypto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-07-26 13:18:01.000000 otgCrypto-0.0.8/otgCrypto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 13:18:01.000000 otgCrypto-0.0.8/otgCrypto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 13:18:01.000000 otgCrypto-0.0.8/otgCrypto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 13:18:01.689163 otgCrypto-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      865 2023-07-26 13:17:57.000000 otgCrypto-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:47:55.785845 otgCrypto-0.0.9/
+-rw-rw-rw-   0        0        0    35821 2023-07-26 09:00:53.000000 otgCrypto-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     3445 2023-07-26 17:47:55.779843 otgCrypto-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2783 2023-07-26 17:43:23.000000 otgCrypto-0.0.9/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 17:47:55.778843 otgCrypto-0.0.9/otgCrypto.egg-info/
+-rw-rw-rw-   0        0        0     3445 2023-07-26 17:47:55.000000 otgCrypto-0.0.9/otgCrypto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-07-26 17:47:55.000000 otgCrypto-0.0.9/otgCrypto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 17:47:55.000000 otgCrypto-0.0.9/otgCrypto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 17:47:55.000000 otgCrypto-0.0.9/otgCrypto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 17:47:55.786843 otgCrypto-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      861 2023-07-26 17:47:48.000000 otgCrypto-0.0.9/setup.py
```

### Comparing `otgCrypto-0.0.8/LICENSE.txt` & `otgCrypto-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `otgCrypto-0.0.8/PKG-INFO` & `otgCrypto-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otgCrypto
-Version: 0.0.8
+Version: 0.0.9
 Summary: OTG cryptography is architectured by Tahsin Ahmed.
 Home-page: 
 Author: Tahsin Ahmed
 Keywords: cryptography,encryption,decryption,otg,otg cryptography,one time gamble,one time gamble cryptography
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
@@ -45,15 +45,15 @@
 
 --------------------------------
 **Caution**
 --------------------------------
 * OTG is a very typo sensitive system.
 * It should be used only for very sensitive work.
 * This cryptography ensures OTC (One Time Chance) method.
-* Message will be deleted if a user give wrong password only at once.
+* Message will be deleted if a user gives wrong password only at once.
 
 --------------------------------
 **Do You Want To Know Me?**
 --------------------------------
 * **Call**: +8801818832925
-* **Email**: tahsin.ahmed@gbracu.ac.bd
+* **Email**: tahsin.ahmed@g.bracu.ac.bd
 * **Facebook**: https://www.facebook.com/ahmedinsider
```

### Comparing `otgCrypto-0.0.8/README.txt` & `otgCrypto-0.0.9/README.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 --------------------------------
 **Caution**
 --------------------------------
 * OTG is a very typo sensitive system.
 * It should be used only for very sensitive work.
 * This cryptography ensures OTC (One Time Chance) method.
-* Message will be deleted if a user give wrong password only at once.
+* Message will be deleted if a user gives wrong password only at once.
 
 --------------------------------
 **Do You Want To Know Me?**
 --------------------------------
 * **Call**: +8801818832925
-* **Email**: tahsin.ahmed@gbracu.ac.bd
+* **Email**: tahsin.ahmed@g.bracu.ac.bd
 * **Facebook**: https://www.facebook.com/ahmedinsider
```

### Comparing `otgCrypto-0.0.8/otgCrypto.egg-info/PKG-INFO` & `otgCrypto-0.0.9/otgCrypto.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otgCrypto
-Version: 0.0.8
+Version: 0.0.9
 Summary: OTG cryptography is architectured by Tahsin Ahmed.
 Home-page: 
 Author: Tahsin Ahmed
 Keywords: cryptography,encryption,decryption,otg,otg cryptography,one time gamble,one time gamble cryptography
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
@@ -45,15 +45,15 @@
 
 --------------------------------
 **Caution**
 --------------------------------
 * OTG is a very typo sensitive system.
 * It should be used only for very sensitive work.
 * This cryptography ensures OTC (One Time Chance) method.
-* Message will be deleted if a user give wrong password only at once.
+* Message will be deleted if a user gives wrong password only at once.
 
 --------------------------------
 **Do You Want To Know Me?**
 --------------------------------
 * **Call**: +8801818832925
-* **Email**: tahsin.ahmed@gbracu.ac.bd
+* **Email**: tahsin.ahmed@g.bracu.ac.bd
 * **Facebook**: https://www.facebook.com/ahmedinsider
```

### Comparing `otgCrypto-0.0.8/setup.py` & `otgCrypto-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "otgCrypto",
-    
-    version = "0.0.8",
+
+    version = "0.0.9",
     
     author = "Tahsin Ahmed",
 
     description = "OTG cryptography is architectured by Tahsin Ahmed.",
 
     long_description = open("README.txt").read(),
```

