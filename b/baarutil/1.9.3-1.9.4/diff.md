# Comparing `tmp/baarutil-1.9.3.tar.gz` & `tmp/baarutil-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\baarutil-1.9.3.tar", last modified: Tue Jul 11 10:02:49 2023, max compression
+gzip compressed data, was "dist\baarutil-1.9.4.tar", last modified: Mon Jul 31 10:56:16 2023, max compression
```

## Comparing `baarutil-1.9.3.tar` & `baarutil-1.9.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 10:02:49.000000 baarutil-1.9.3/
--rw-rw-rw-   0        0        0    24131 2023-07-11 10:02:49.000000 baarutil-1.9.3/PKG-INFO
--rw-rw-rw-   0        0        0    19458 2023-07-11 10:01:38.000000 baarutil-1.9.3/README.md
--rw-rw-rw-   0        0        0      108 2022-05-17 16:01:08.000000 baarutil-1.9.3/pyproject.toml
--rw-rw-rw-   0        0        0      866 2023-07-11 10:02:49.000000 baarutil-1.9.3/setup.cfg
--rw-rw-rw-   0        0        0     1139 2023-07-11 09:55:49.000000 baarutil-1.9.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:02:47.000000 baarutil-1.9.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 10:02:49.000000 baarutil-1.9.3/src/baarutil/
--rw-rw-rw-   0        0        0       32 2022-11-04 10:25:03.000000 baarutil-1.9.3/src/baarutil/__init__.py
--rw-rw-rw-   0        0        0    11242 2023-03-08 14:02:35.000000 baarutil-1.9.3/src/baarutil/baarlocker.py
--rw-rw-rw-   0        0        0     2828 2023-03-08 14:09:20.000000 baarutil-1.9.3/src/baarutil/chromedriver_downloader.py
--rw-rw-rw-   0        0        0    30067 2023-07-11 09:41:40.000000 baarutil-1.9.3/src/baarutil/converter.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:02:49.000000 baarutil-1.9.3/src/baarutil.egg-info/
--rw-rw-rw-   0        0        0    24131 2023-07-11 10:02:47.000000 baarutil-1.9.3/src/baarutil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-07-11 10:02:47.000000 baarutil-1.9.3/src/baarutil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 10:02:47.000000 baarutil-1.9.3/src/baarutil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      154 2023-07-11 10:02:47.000000 baarutil-1.9.3/src/baarutil.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-11 10:02:47.000000 baarutil-1.9.3/src/baarutil.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 10:56:16.000000 baarutil-1.9.4/
+-rw-rw-rw-   0        0        0    24512 2023-07-31 10:56:16.000000 baarutil-1.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0    19823 2023-07-31 10:39:15.000000 baarutil-1.9.4/README.md
+-rw-rw-rw-   0        0        0      108 2022-05-17 16:01:08.000000 baarutil-1.9.4/pyproject.toml
+-rw-rw-rw-   0        0        0      866 2023-07-31 10:56:16.000000 baarutil-1.9.4/setup.cfg
+-rw-rw-rw-   0        0        0     1139 2023-07-31 10:31:05.000000 baarutil-1.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 10:56:16.000000 baarutil-1.9.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 10:56:16.000000 baarutil-1.9.4/src/baarutil/
+-rw-rw-rw-   0        0        0       32 2022-11-04 10:25:03.000000 baarutil-1.9.4/src/baarutil/__init__.py
+-rw-rw-rw-   0        0        0    11242 2023-03-08 14:02:35.000000 baarutil-1.9.4/src/baarutil/baarlocker.py
+-rw-rw-rw-   0        0        0     2828 2023-03-08 14:09:20.000000 baarutil-1.9.4/src/baarutil/chromedriver_downloader.py
+-rw-rw-rw-   0        0        0    30651 2023-07-31 10:20:02.000000 baarutil-1.9.4/src/baarutil/converter.py
+drwxrwxrwx   0        0        0        0 2023-07-31 10:56:16.000000 baarutil-1.9.4/src/baarutil.egg-info/
+-rw-rw-rw-   0        0        0    24512 2023-07-31 10:56:16.000000 baarutil-1.9.4/src/baarutil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-07-31 10:56:16.000000 baarutil-1.9.4/src/baarutil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 10:56:16.000000 baarutil-1.9.4/src/baarutil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      154 2023-07-31 10:56:16.000000 baarutil-1.9.4/src/baarutil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 10:56:16.000000 baarutil-1.9.4/src/baarutil.egg-info/top_level.txt
```

### Comparing `baarutil-1.9.3/PKG-INFO` & `baarutil-1.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: baarutil
-Version: 1.9.3
+Version: 1.9.4
 Summary: Utility functions for BAAR developers
 Home-page: https://github.com/Allied-Media/baarutil
 Author: Souvik Roy
 Author-email: souvik.roy@alliedmedia.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Allied-Media/baarutil/issues
 Description: # BAARUtil
         
-        **Version: 1.9.3**
+        **Version: 1.9.4**
         
-        Minor Update - Contains bug fixes.
+        Minor Update - Contains enhancement.
         
-        Details: df_to_string() function now supports latest pandas versions (*i.e. pandas==2.0.3*)
+        Details: generate_password() function now has a new argument "include_chars" where the user can provide the list of characters among which at leas one must be included in the final password.
         
         **This Custom Library is specifically created for the developers/users who use BAAR. Which is a product of [BAAR Technologies](https://www.baar.ai/) aka [Allied Media Inc](https://www.alliedmedia.com/).**
         
         <h2>
         Primary Author and Contributor:
         </h2>
         
         **Souvik Roy  [sroy-2019](https://github.com/sroy-2019)**
         
         <h3>
         Co-contributors:
         </h3>
         
-        **Saikat Dey**
-        **Debapriya Palai**
+        **Saikat Dey,**
+        **Debapriya Palai,**
         **Avignan Nag**
         
         <h2>
         Installation:
         </h2>
         
         ~~~
@@ -261,18 +261,20 @@
         
           *ii. **upper:**  Are Uppercase characters required?, Data Type = Bool (True/False), Default Value = True*
         
           *iii. **lower:**  Are Lowercase characters required?, Data Type = Bool (True/False), Default Value = True*
         
           *iv. **digits:**  Are Digits characters required?, Data Type = Bool (True/False), Default Value = True*
         
-          *v. **symbols:**  Are Symbols/ Special characters required?, Data Type = Bool (True/False), Default Value = True*
+          *v. **symbols:**  Are Symbols/ Special characters required?, Data Type = Bool (True/False), Default Value = True, Built-in available values: ['@', '#', '$', '%', '=', ':', '?', '.', '/', '|', '~', '>', '\*', '(', ')', '<']*
         
           *vi. **exclude_chars:**  List of characters to be excluded from the final password, Data Type = List, Default Value = []*
         
+          *vii. **include_chars:**  List of characters from which at least one must be included in the final password, Data Type = List, Default Value = []*
+        
           This function can also be called from a Robot Framework Script by importing the baarutil library and using Generate Password keyword. Upon initiation of this function, this will set the Log Level of the Robot Framework script to NONE for security reasons. The Developers have to use *Set Log Level    INFO* in the robot script in order to restart the Log.
         
         ~~~
         Input (Optional):  <<Password Length>>, <<Uppercase Required?>>, <<Lowercase Required?>>, <<Digits Required?>>, <<Symbols Required?>>
         Output: <<Password String>>
         ~~~
```

### Comparing `baarutil-1.9.3/README.md` & `baarutil-1.9.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # BAARUtil
 
-**Version: 1.9.3**
+**Version: 1.9.4**
 
-Minor Update - Contains bug fixes.
+Minor Update - Contains enhancement.
 
-Details: df_to_string() function now supports latest pandas versions (*i.e. pandas==2.0.3*)
+Details: generate_password() function now has a new argument "include_chars" where the user can provide the list of characters among which at leas one must be included in the final password.
 
 **This Custom Library is specifically created for the developers/users who use BAAR. Which is a product of [BAAR Technologies](https://www.baar.ai/) aka [Allied Media Inc](https://www.alliedmedia.com/).**
 
 <h2>
 Primary Author and Contributor:
 </h2>
 
 **Souvik Roy  [sroy-2019](https://github.com/sroy-2019)**
 
 <h3>
 Co-contributors:
 </h3>
 
-**Saikat Dey**
-**Debapriya Palai**
+**Saikat Dey,**
+**Debapriya Palai,**
 **Avignan Nag**
 
 <h2>
 Installation:
 </h2>
 
 ~~~
@@ -252,18 +252,20 @@
 
   *ii. **upper:**  Are Uppercase characters required?, Data Type = Bool (True/False), Default Value = True*
 
   *iii. **lower:**  Are Lowercase characters required?, Data Type = Bool (True/False), Default Value = True*
 
   *iv. **digits:**  Are Digits characters required?, Data Type = Bool (True/False), Default Value = True*
 
-  *v. **symbols:**  Are Symbols/ Special characters required?, Data Type = Bool (True/False), Default Value = True*
+  *v. **symbols:**  Are Symbols/ Special characters required?, Data Type = Bool (True/False), Default Value = True, Built-in available values: ['@', '#', '$', '%', '=', ':', '?', '.', '/', '|', '~', '>', '\*', '(', ')', '<']*
 
   *vi. **exclude_chars:**  List of characters to be excluded from the final password, Data Type = List, Default Value = []*
 
+  *vii. **include_chars:**  List of characters from which at least one must be included in the final password, Data Type = List, Default Value = []*
+
   This function can also be called from a Robot Framework Script by importing the baarutil library and using Generate Password keyword. Upon initiation of this function, this will set the Log Level of the Robot Framework script to NONE for security reasons. The Developers have to use *Set Log Level    INFO* in the robot script in order to restart the Log.
 
 ~~~
 Input (Optional):  <<Password Length>>, <<Uppercase Required?>>, <<Lowercase Required?>>, <<Digits Required?>>, <<Symbols Required?>>
 Output: <<Password String>>
 ~~~
```

#### html2text {}

```diff
@@ -1,16 +1,18 @@
-# BAARUtil **Version: 1.9.3** Minor Update - Contains bug fixes. Details:
-df_to_string() function now supports latest pandas versions (*i.e.
-pandas==2.0.3*) **This Custom Library is specifically created for the
-developers/users who use BAAR. Which is a product of [BAAR Technologies](https:
-//www.baar.ai/) aka [Allied Media Inc](https://www.alliedmedia.com/).**
+# BAARUtil **Version: 1.9.4** Minor Update - Contains enhancement. Details:
+generate_password() function now has a new argument "include_chars" where the
+user can provide the list of characters among which at leas one must be
+included in the final password. **This Custom Library is specifically created
+for the developers/users who use BAAR. Which is a product of [BAAR
+Technologies](https://www.baar.ai/) aka [Allied Media Inc](https://
+www.alliedmedia.com/).**
 ***** Primary Author and Contributor: *****
 **Souvik Roy [sroy-2019](https://github.com/sroy-2019)**
 **** Co-contributors: ****
-**Saikat Dey** **Debapriya Palai** **Avignan Nag**
+**Saikat Dey,** **Debapriya Palai,** **Avignan Nag**
 ***** Installation: *****
 ~~~ pip install baarutil ~~~
 ***** Importing: *****
 ~~~ import baarutil as bu ~~~
 ***** Additional Info: *****
 The string structure that follows is a streamlined structure that the
 developers/users follow throughout an automation workflow designed in BAAR: ~~~
@@ -92,21 +94,24 @@
 **Attributes:** *i. **password_size:** Password Length, Data Type = int,
 Default Value = 10, (Should be greater than 4)* *ii. **upper:** Are Uppercase
 characters required?, Data Type = Bool (True/False), Default Value = True*
 *iii. **lower:** Are Lowercase characters required?, Data Type = Bool (True/
 False), Default Value = True* *iv. **digits:** Are Digits characters required?,
 Data Type = Bool (True/False), Default Value = True* *v. **symbols:** Are
 Symbols/ Special characters required?, Data Type = Bool (True/False), Default
-Value = True* *vi. **exclude_chars:** List of characters to be excluded from
-the final password, Data Type = List, Default Value = []* This function can
-also be called from a Robot Framework Script by importing the baarutil library
-and using Generate Password keyword. Upon initiation of this function, this
-will set the Log Level of the Robot Framework script to NONE for security
-reasons. The Developers have to use *Set Log Level INFO* in the robot script in
-order to restart the Log. ~~~ Input (Optional): <>, <
+Value = True, Built-in available values: ['@', '#', '$', '%', '=', ':', '?',
+'.', '/', '|', '~', '>', '\*', '(', ')', '<']* *vi. **exclude_chars:** List of
+characters to be excluded from the final password, Data Type = List, Default
+Value = []* *vii. **include_chars:** List of characters from which at least one
+must be included in the final password, Data Type = List, Default Value = []*
+This function can also be called from a Robot Framework Script by importing the
+baarutil library and using Generate Password keyword. Upon initiation of this
+function, this will set the Log Level of the Robot Framework script to NONE for
+security reasons. The Developers have to use *Set Log Level INFO* in the robot
+script in order to restart the Log. ~~~ Input (Optional): <>, <
 >>, <
 >>, <
 >>, <
 >> Output: <> ~~~
 d="generate_report"> 8. Function: generate_report(data_df, file_name, path,
 file_type, detailed_report, replace_old_file, final_file_name_case, time_stamp,
 encoding, index, engine, max_new_files_count, sheet_name), Output Data Type:
```

### Comparing `baarutil-1.9.3/setup.cfg` & `baarutil-1.9.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 6161 7275 7469 6c0d 0a76 6572   = baarutil..ver
-00000020: 7369 6f6e 203d 2031 2e39 2e33 0d0a 6175  sion = 1.9.3..au
+00000020: 7369 6f6e 203d 2031 2e39 2e34 0d0a 6175  sion = 1.9.4..au
 00000030: 7468 6f72 203d 2053 6f75 7669 6b20 526f  thor = Souvik Ro
 00000040: 790d 0a61 7574 686f 725f 656d 6169 6c20  y..author_email 
 00000050: 3d20 736f 7576 696b 2e72 6f79 4061 6c6c  = souvik.roy@all
 00000060: 6965 646d 6564 6961 2e63 6f6d 0d0a 6465  iedmedia.com..de
 00000070: 7363 7269 7074 696f 6e20 3d20 5574 696c  scription = Util
 00000080: 6974 7920 6675 6e63 7469 6f6e 7320 666f  ity functions fo
 00000090: 7220 4241 4152 2064 6576 656c 6f70 6572  r BAAR developer
```

### Comparing `baarutil-1.9.3/setup.py` & `baarutil-1.9.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="baarutil",
-    version="1.9.3",
+    version="1.9.4",
     author="Souvik Roy",
     author_email="souvik.roy@alliedmedia.com",
     description="Utility functions for BAAR developers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Allied-Media/baarutil",
     project_urls={
```

### Comparing `baarutil-1.9.3/src/baarutil/baarlocker.py` & `baarutil-1.9.4/src/baarutil/baarlocker.py`

 * *Files identical despite different names*

### Comparing `baarutil-1.9.3/src/baarutil/chromedriver_downloader.py` & `baarutil-1.9.4/src/baarutil/chromedriver_downloader.py`

 * *Files identical despite different names*

### Comparing `baarutil-1.9.3/src/baarutil/converter.py` & `baarutil-1.9.4/src/baarutil/converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import array
 import datetime
 import shutil
 import baarutil.chromedriver_downloader as cdl
 
 
 # Version info
-curr_version = r'1.9.2'
+curr_version = r'1.9.4'
 
 
 def version() -> str:
     """This function returns the version of the BAARUtil"""
     global curr_version
     return curr_version
 
@@ -232,15 +232,15 @@
     except Exception as e:
         print('Decryption failed! Incorrect Encrypted data.', flush=True)
         print(traceback.format_exc(), flush=True)
     return decrypted_string
 
 
 @keyword("Generate Password")
-def generate_password(password_size: int = 10, upper: bool = True, lower: bool = True, digits: bool = True, symbols: bool = True, exclude_chars: list = []) -> str:
+def generate_password(password_size: int = 10, upper: bool = True, lower: bool = True, digits: bool = True, symbols: bool = True, exclude_chars: list = [], include_chars: list = []) -> str:
     """This function generates random Passwords"""
     try:
         # This will set the Log Level to NONE if it is called from a Robot Framework script
         BuiltIn.log_to_console(
             BuiltIn(), 'Setting Log Level from INFO to NONE!')
         old = _Misc.set_log_level(_Misc(), level='NONE')
     except:
@@ -261,27 +261,33 @@
     DIGITS = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
     LOCASE_CHARACTERS = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k',
                          'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']
     UPCASE_CHARACTERS = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K',
                          'M', 'N', 'O', 'p', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
     SYMBOLS = ['@', '#', '$', '%', '=', ':', '?',
                '.', '/', '|', '~', '>', '*', '(', ')', '<']
-    rand_digit = rand_upper = rand_lower = rand_symbol = ''
+    required_chars = False
+    if len(include_chars) > 0:
+        min_password_size = 5
+        required_chars = True
+    else:
+        min_password_size = 4
+    rand_digit = rand_upper = rand_lower = rand_symbol = rand_include_chars = ''
     final_combined_list = []
     default_count = 0
 
     # ~~~~ Applying exclusion list ~~~~
     DIGITS = apply_exclusion_list(DIGITS, exclude_chars)
     LOCASE_CHARACTERS = apply_exclusion_list(LOCASE_CHARACTERS, exclude_chars)
     UPCASE_CHARACTERS = apply_exclusion_list(UPCASE_CHARACTERS, exclude_chars)
     SYMBOLS = apply_exclusion_list(SYMBOLS, exclude_chars)
 
     # ~~~~ Main Operation ~~~~
     try:
-        if not password_size < 4:
+        if not password_size < min_password_size:
             if upper:
                 final_combined_list += UPCASE_CHARACTERS
                 rand_upper = random.choice(UPCASE_CHARACTERS)
                 default_count += 1
             if lower:
                 final_combined_list += LOCASE_CHARACTERS
                 rand_lower = random.choice(LOCASE_CHARACTERS)
@@ -290,18 +296,25 @@
                 final_combined_list += DIGITS
                 rand_digit = random.choice(DIGITS)
                 default_count += 1
             if symbols:
                 final_combined_list += SYMBOLS
                 rand_symbol = random.choice(SYMBOLS)
                 default_count += 1
+            if required_chars:
+                final_combined_list += include_chars
+                rand_include_chars = random.choice(include_chars)
+                default_count += 1
 
             if upper or lower or digits or symbols:
                 COMBINED_LIST = final_combined_list
-                temp_pass = rand_digit + rand_upper + rand_lower + rand_symbol
+                if required_chars:
+                    temp_pass = rand_digit + rand_upper + rand_lower + rand_symbol + rand_include_chars
+                else:
+                    temp_pass = rand_digit + rand_upper + rand_lower + rand_symbol
                 temp_pass_list = []
                 for count in range(MAX_LEN - default_count):
                     temp_pass = temp_pass + random.choice(COMBINED_LIST)
                     temp_pass_list = array.array('u', temp_pass)
                     random.shuffle(temp_pass_list)
                 for char in temp_pass_list:
                     password = password + char
```

### Comparing `baarutil-1.9.3/src/baarutil.egg-info/PKG-INFO` & `baarutil-1.9.4/src/baarutil.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: baarutil
-Version: 1.9.3
+Version: 1.9.4
 Summary: Utility functions for BAAR developers
 Home-page: https://github.com/Allied-Media/baarutil
 Author: Souvik Roy
 Author-email: souvik.roy@alliedmedia.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Allied-Media/baarutil/issues
 Description: # BAARUtil
         
-        **Version: 1.9.3**
+        **Version: 1.9.4**
         
-        Minor Update - Contains bug fixes.
+        Minor Update - Contains enhancement.
         
-        Details: df_to_string() function now supports latest pandas versions (*i.e. pandas==2.0.3*)
+        Details: generate_password() function now has a new argument "include_chars" where the user can provide the list of characters among which at leas one must be included in the final password.
         
         **This Custom Library is specifically created for the developers/users who use BAAR. Which is a product of [BAAR Technologies](https://www.baar.ai/) aka [Allied Media Inc](https://www.alliedmedia.com/).**
         
         <h2>
         Primary Author and Contributor:
         </h2>
         
         **Souvik Roy  [sroy-2019](https://github.com/sroy-2019)**
         
         <h3>
         Co-contributors:
         </h3>
         
-        **Saikat Dey**
-        **Debapriya Palai**
+        **Saikat Dey,**
+        **Debapriya Palai,**
         **Avignan Nag**
         
         <h2>
         Installation:
         </h2>
         
         ~~~
@@ -261,18 +261,20 @@
         
           *ii. **upper:**  Are Uppercase characters required?, Data Type = Bool (True/False), Default Value = True*
         
           *iii. **lower:**  Are Lowercase characters required?, Data Type = Bool (True/False), Default Value = True*
         
           *iv. **digits:**  Are Digits characters required?, Data Type = Bool (True/False), Default Value = True*
         
-          *v. **symbols:**  Are Symbols/ Special characters required?, Data Type = Bool (True/False), Default Value = True*
+          *v. **symbols:**  Are Symbols/ Special characters required?, Data Type = Bool (True/False), Default Value = True, Built-in available values: ['@', '#', '$', '%', '=', ':', '?', '.', '/', '|', '~', '>', '\*', '(', ')', '<']*
         
           *vi. **exclude_chars:**  List of characters to be excluded from the final password, Data Type = List, Default Value = []*
         
+          *vii. **include_chars:**  List of characters from which at least one must be included in the final password, Data Type = List, Default Value = []*
+        
           This function can also be called from a Robot Framework Script by importing the baarutil library and using Generate Password keyword. Upon initiation of this function, this will set the Log Level of the Robot Framework script to NONE for security reasons. The Developers have to use *Set Log Level    INFO* in the robot script in order to restart the Log.
         
         ~~~
         Input (Optional):  <<Password Length>>, <<Uppercase Required?>>, <<Lowercase Required?>>, <<Digits Required?>>, <<Symbols Required?>>
         Output: <<Password String>>
         ~~~
```

