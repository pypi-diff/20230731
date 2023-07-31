# Comparing `tmp/email_extractor_unicode-1.0.6.tar.gz` & `tmp/email_extractor_unicode-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "email_extractor_unicode-1.0.6.tar", last modified: Mon Jul 31 08:17:15 2023, max compression
+gzip compressed data, was "email_extractor_unicode-1.0.7.tar", last modified: Mon Jul 31 09:54:45 2023, max compression
```

## Comparing `email_extractor_unicode-1.0.6.tar` & `email_extractor_unicode-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 08:17:15.183079 email_extractor_unicode-1.0.6/
--rw-rw-rw-   0        0        0     1137 2023-07-31 06:42:12.000000 email_extractor_unicode-1.0.6/LICENSE.rst
--rw-rw-rw-   0        0        0     3952 2023-07-31 08:17:15.182039 email_extractor_unicode-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2272 2023-07-31 08:16:38.000000 email_extractor_unicode-1.0.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-31 08:17:15.150038 email_extractor_unicode-1.0.6/email_extractor_unicode/
--rw-rw-rw-   0        0        0       55 2023-07-31 07:13:06.000000 email_extractor_unicode-1.0.6/email_extractor_unicode/__init__.py
--rw-rw-rw-   0        0        0     2780 2023-07-31 08:14:25.000000 email_extractor_unicode-1.0.6/email_extractor_unicode/extractor.py
-drwxrwxrwx   0        0        0        0 2023-07-31 08:17:15.178054 email_extractor_unicode-1.0.6/email_extractor_unicode.egg-info/
--rw-rw-rw-   0        0        0     3952 2023-07-31 08:17:14.000000 email_extractor_unicode-1.0.6/email_extractor_unicode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-07-31 08:17:15.000000 email_extractor_unicode-1.0.6/email_extractor_unicode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 08:17:14.000000 email_extractor_unicode-1.0.6/email_extractor_unicode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-31 08:17:14.000000 email_extractor_unicode-1.0.6/email_extractor_unicode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-07-31 08:17:14.000000 email_extractor_unicode-1.0.6/email_extractor_unicode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 08:17:15.183079 email_extractor_unicode-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1061 2023-07-31 08:16:31.000000 email_extractor_unicode-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:54:45.411508 email_extractor_unicode-1.0.7/
+-rw-rw-rw-   0        0        0     1137 2023-07-31 06:42:12.000000 email_extractor_unicode-1.0.7/LICENSE.rst
+-rw-rw-rw-   0        0        0     3833 2023-07-31 09:54:45.410222 email_extractor_unicode-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2153 2023-07-31 09:54:11.000000 email_extractor_unicode-1.0.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-31 09:54:45.352110 email_extractor_unicode-1.0.7/email_extractor_unicode/
+-rw-rw-rw-   0        0        0       55 2023-07-31 09:54:15.000000 email_extractor_unicode-1.0.7/email_extractor_unicode/__init__.py
+-rw-rw-rw-   0        0        0     2861 2023-07-31 09:54:17.000000 email_extractor_unicode-1.0.7/email_extractor_unicode/extractor.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:54:45.407223 email_extractor_unicode-1.0.7/email_extractor_unicode.egg-info/
+-rw-rw-rw-   0        0        0     3833 2023-07-31 09:54:45.000000 email_extractor_unicode-1.0.7/email_extractor_unicode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-07-31 09:54:45.000000 email_extractor_unicode-1.0.7/email_extractor_unicode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 09:54:45.000000 email_extractor_unicode-1.0.7/email_extractor_unicode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-31 09:54:45.000000 email_extractor_unicode-1.0.7/email_extractor_unicode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-07-31 09:54:45.000000 email_extractor_unicode-1.0.7/email_extractor_unicode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 09:54:45.411508 email_extractor_unicode-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1061 2023-07-31 09:54:20.000000 email_extractor_unicode-1.0.7/setup.py
```

### Comparing `email_extractor_unicode-1.0.6/LICENSE.rst` & `email_extractor_unicode-1.0.7/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `email_extractor_unicode-1.0.6/PKG-INFO` & `email_extractor_unicode-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: email_extractor_unicode
-Version: 1.0.6
+Version: 1.0.7
 Summary: Extract Emails Using Phone Number
 Home-page: https://t.me/iamunicode
 Author: Unicode
 License: MIT
 Keywords: emails
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
@@ -51,20 +51,18 @@
 <p>Please use this library responsibly and respect the terms of service of the websites you are scraping. Email
    extraction from websites may be subject to legal restrictions in some jurisdictions. Always ensure you have the
    right to extract data from the websites you visit.
 </p>
 
 <h2>Change Log</h2>
 <ul>
-    <li><strong>1.0.6 (07/31/2023)</strong></li>
+    <li><strong>1.0.7 (07/31/2023)</strong></li>
     <ul>
         <li>Second Release</li>
-        <li>Fixed: line 63, in extract_emails_from_phone_file<br>
-        driver.quit()<br>
-        UnboundLocalError: local variable 'driver' referenced before assignment</li>
+        <li>Fixed: Remove +1 if exists in phone number</li>
     </ul>
 </ul>
 
 
 <h2>License</h2>
 
 <p>Copyright 2023 UNICODE</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: email_extractor_unicode Version: 1.0.6 Summary:
+Metadata-Version: 2.1 Name: email_extractor_unicode Version: 1.0.7 Summary:
 Extract Emails Using Phone Number Home-page: https://t.me/iamunicode Author:
 Unicode License: MIT Keywords: emails Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Education Classifier:
 Operating System :: Microsoft :: Windows :: Windows 10 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown License-File: LICENSE.rst
 ****** Email Extractor Unicode ******
@@ -38,20 +38,17 @@
 issues related to Email Extractor Unicode.
 ***** Disclaimer *****
 Please use this library responsibly and respect the terms of service of the
 websites you are scraping. Email extraction from websites may be subject to
 legal restrictions in some jurisdictions. Always ensure you have the right to
 extract data from the websites you visit.
 ***** Change Log *****
-    * 1.0.6 (07/31/2023)
+    * 1.0.7 (07/31/2023)
           o Second Release
-          o Fixed: line 63, in extract_emails_from_phone_file
-            driver.quit()
-            UnboundLocalError: local variable 'driver' referenced before
-            assignment
+          o Fixed: Remove +1 if exists in phone number
 ***** License *****
 Copyright 2023 UNICODE
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
```

### Comparing `email_extractor_unicode-1.0.6/README.rst` & `email_extractor_unicode-1.0.7/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -35,15 +35,13 @@
 <p>Please use this library responsibly and respect the terms of service of the websites you are scraping. Email
    extraction from websites may be subject to legal restrictions in some jurisdictions. Always ensure you have the
    right to extract data from the websites you visit.
 </p>
 
 <h2>Change Log</h2>
 <ul>
-    <li><strong>1.0.6 (07/31/2023)</strong></li>
+    <li><strong>1.0.7 (07/31/2023)</strong></li>
     <ul>
         <li>Second Release</li>
-        <li>Fixed: line 63, in extract_emails_from_phone_file<br>
-        driver.quit()<br>
-        UnboundLocalError: local variable 'driver' referenced before assignment</li>
+        <li>Fixed: Remove +1 if exists in phone number</li>
     </ul>
 </ul>
```

#### html2text {}

```diff
@@ -31,13 +31,10 @@
 issues related to Email Extractor Unicode.
 ***** Disclaimer *****
 Please use this library responsibly and respect the terms of service of the
 websites you are scraping. Email extraction from websites may be subject to
 legal restrictions in some jurisdictions. Always ensure you have the right to
 extract data from the websites you visit.
 ***** Change Log *****
-    * 1.0.6 (07/31/2023)
+    * 1.0.7 (07/31/2023)
           o Second Release
-          o Fixed: line 63, in extract_emails_from_phone_file
-            driver.quit()
-            UnboundLocalError: local variable 'driver' referenced before
-            assignment
+          o Fixed: Remove +1 if exists in phone number
```

### Comparing `email_extractor_unicode-1.0.6/email_extractor_unicode/extractor.py` & `email_extractor_unicode-1.0.7/email_extractor_unicode/extractor.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,16 @@
             phone_numbers = [phone.strip() for phone in file.readlines()]
 
         # Initialize a set to store all emails without duplicates
         all_emails = set()
 
         # Loop through each phone number, visit the corresponding URL, and extract emails
         for phone in phone_numbers:
+            if "+1" in phone:
+                phone = phone.replace("+1" , "")
             try:
                 url = f'https://www.smartbackgroundchecks.com/phone/{phone}'
                 driver.get(url)
 
                 # Get the page source
                 page_source = driver.page_source
```

### Comparing `email_extractor_unicode-1.0.6/email_extractor_unicode.egg-info/PKG-INFO` & `email_extractor_unicode-1.0.7/email_extractor_unicode.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: email-extractor-unicode
-Version: 1.0.6
+Version: 1.0.7
 Summary: Extract Emails Using Phone Number
 Home-page: https://t.me/iamunicode
 Author: Unicode
 License: MIT
 Keywords: emails
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
@@ -51,20 +51,18 @@
 <p>Please use this library responsibly and respect the terms of service of the websites you are scraping. Email
    extraction from websites may be subject to legal restrictions in some jurisdictions. Always ensure you have the
    right to extract data from the websites you visit.
 </p>
 
 <h2>Change Log</h2>
 <ul>
-    <li><strong>1.0.6 (07/31/2023)</strong></li>
+    <li><strong>1.0.7 (07/31/2023)</strong></li>
     <ul>
         <li>Second Release</li>
-        <li>Fixed: line 63, in extract_emails_from_phone_file<br>
-        driver.quit()<br>
-        UnboundLocalError: local variable 'driver' referenced before assignment</li>
+        <li>Fixed: Remove +1 if exists in phone number</li>
     </ul>
 </ul>
 
 
 <h2>License</h2>
 
 <p>Copyright 2023 UNICODE</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: email-extractor-unicode Version: 1.0.6 Summary:
+Metadata-Version: 2.1 Name: email-extractor-unicode Version: 1.0.7 Summary:
 Extract Emails Using Phone Number Home-page: https://t.me/iamunicode Author:
 Unicode License: MIT Keywords: emails Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Education Classifier:
 Operating System :: Microsoft :: Windows :: Windows 10 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown License-File: LICENSE.rst
 ****** Email Extractor Unicode ******
@@ -38,20 +38,17 @@
 issues related to Email Extractor Unicode.
 ***** Disclaimer *****
 Please use this library responsibly and respect the terms of service of the
 websites you are scraping. Email extraction from websites may be subject to
 legal restrictions in some jurisdictions. Always ensure you have the right to
 extract data from the websites you visit.
 ***** Change Log *****
-    * 1.0.6 (07/31/2023)
+    * 1.0.7 (07/31/2023)
           o Second Release
-          o Fixed: line 63, in extract_emails_from_phone_file
-            driver.quit()
-            UnboundLocalError: local variable 'driver' referenced before
-            assignment
+          o Fixed: Remove +1 if exists in phone number
 ***** License *****
 Copyright 2023 UNICODE
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
```

### Comparing `email_extractor_unicode-1.0.6/setup.py` & `email_extractor_unicode-1.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 with open('LICENSE.rst', encoding='utf-8') as license_file:
     license_content = license_file.read()
 
 
 setup(
     name='email_extractor_unicode',
-    version='1.0.6',
+    version='1.0.7',
     description='Extract Emails Using Phone Number',
     long_description=readme_content + '\n\n' + license_content,
     long_description_content_type='text/markdown',  # Specify the content type as reStructuredText
     url='https://t.me/iamunicode',
     author='Unicode',
     license='MIT',
     classifiers=classifiers,
```

