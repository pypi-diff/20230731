# Comparing `tmp/py_auth_micro-0.1.6.tar.gz` & `tmp/py_auth_micro-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_auth_micro-0.1.6.tar", last modified: Tue May 23 07:09:13 2023, max compression
+gzip compressed data, was "py_auth_micro-0.1.7.tar", last modified: Mon Jul 31 13:48:20 2023, max compression
```

## Comparing `py_auth_micro-0.1.6.tar` & `py_auth_micro-0.1.7.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:09:13.384435 py_auth_micro-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-23 07:09:13.384435 py_auth_micro-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:09:13.380435 py_auth_micro-0.1.6/py_auth_micro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:09:13.384435 py_auth_micro-0.1.6/py_auth_micro/Config/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/Config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/Config/_appconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/Config/_dbconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/Config/_ldapconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:09:13.384435 py_auth_micro-0.1.6/py_auth_micro/Core/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/Core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/Core/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/Core/_ldap_interactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:09:13.384435 py_auth_micro-0.1.6/py_auth_micro/Exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/Exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:09:13.384435 py_auth_micro-0.1.6/py_auth_micro/LoginHandler/
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/LoginHandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/LoginHandler/_loginbaseclass.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/LoginHandler/_loginkerberos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/LoginHandler/_loginldap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/LoginHandler/_loginlocal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:09:13.384435 py_auth_micro-0.1.6/py_auth_micro/Models/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/Models/_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/Models/_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/Models/_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:09:13.384435 py_auth_micro-0.1.6/py_auth_micro/WorkFlows/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/WorkFlows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/WorkFlows/_groupworkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/WorkFlows/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/WorkFlows/_sessionworkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/WorkFlows/_userworkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/py_auth_micro/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:09:13.384435 py_auth_micro-0.1.6/py_auth_micro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-23 07:09:13.000000 py_auth_micro-0.1.6/py_auth_micro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-23 07:09:13.000000 py_auth_micro-0.1.6/py_auth_micro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 07:09:13.000000 py_auth_micro-0.1.6/py_auth_micro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-23 07:09:13.000000 py_auth_micro-0.1.6/py_auth_micro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 07:09:13.000000 py_auth_micro-0.1.6/py_auth_micro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-23 07:09:13.384435 py_auth_micro-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-23 07:08:30.000000 py_auth_micro-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:48:20.970367 py_auth_micro-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-31 13:48:20.970367 py_auth_micro-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:48:20.966367 py_auth_micro-0.1.7/py_auth_micro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:48:20.966367 py_auth_micro-0.1.7/py_auth_micro/Config/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/py_auth_micro/Config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/py_auth_micro/Config/_appconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/py_auth_micro/Config/_dbconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/py_auth_micro/Config/_ldapconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:48:20.970367 py_auth_micro-0.1.7/py_auth_micro/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/py_auth_micro/Core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/py_auth_micro/Core/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/py_auth_micro/Core/_ldap_interactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:48:20.970367 py_auth_micro-0.1.7/py_auth_micro/Exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/py_auth_micro/Exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:48:20.970367 py_auth_micro-0.1.7/py_auth_micro/LoginHandler/
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/py_auth_micro/LoginHandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/py_auth_micro/LoginHandler/_loginbaseclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/py_auth_micro/LoginHandler/_loginldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/py_auth_micro/LoginHandler/_loginlocal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:48:20.970367 py_auth_micro-0.1.7/py_auth_micro/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/py_auth_micro/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/py_auth_micro/Models/_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/py_auth_micro/Models/_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/py_auth_micro/Models/_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:48:20.970367 py_auth_micro-0.1.7/py_auth_micro/WorkFlows/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/py_auth_micro/WorkFlows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/py_auth_micro/WorkFlows/_groupworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/py_auth_micro/WorkFlows/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/py_auth_micro/WorkFlows/_sessionworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/py_auth_micro/WorkFlows/_userworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/py_auth_micro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/py_auth_micro/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:48:20.966367 py_auth_micro-0.1.7/py_auth_micro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-31 13:48:20.000000 py_auth_micro-0.1.7/py_auth_micro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-31 13:48:20.000000 py_auth_micro-0.1.7/py_auth_micro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 13:48:20.000000 py_auth_micro-0.1.7/py_auth_micro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-31 13:48:20.000000 py_auth_micro-0.1.7/py_auth_micro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-31 13:48:20.000000 py_auth_micro-0.1.7/py_auth_micro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-31 13:48:20.970367 py_auth_micro-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-31 13:47:39.000000 py_auth_micro-0.1.7/setup.py
```

### Comparing `py_auth_micro-0.1.6/LICENSE` & `py_auth_micro-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.6/PKG-INFO` & `py_auth_micro-0.1.7/py_auth_micro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py_auth_micro
-Version: 0.1.6
+Name: py-auth-micro
+Version: 0.1.7
 Summary: A wrapper around pyjwt
 Home-page: https://github.com/bad-microservices/py_auth_micro
 Author: Ole Hannemann
 Author-email: cerberus885@gmail.com
 License: MIT
 Keywords: JWT
 Classifier: Programming Language :: Python :: 3.0
@@ -19,15 +19,15 @@
 py_auth_micro
 ================
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://pypi.org/project/black
 
 .. image:: https://app.codacy.com/project/badge/Grade/199fd463ff1a487eb206a2afbfb25168
-    :target: https://www.codacy.com/gh/bad-microservices/py_auth_micro/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=bad-microservices/py_auth_micro&amp;utm_campaign=Badge_Grade
+    :target: https://app.codacy.com/gh/bad-microservices/py_auth_micro/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
 
 .. image:: https://badge.fury.io/py/py-auth-micro.svg
     :target: https://badge.fury.io/py/py-auth-micro
 
 .. image:: https://github.com/bad-microservices/py_auth_micro/actions/workflows/documentation.yaml/badge.svg
    :target: https://github.com/bad-microservices/py_auth_micro/actions?query=workflow:Docs
```

### Comparing `py_auth_micro-0.1.6/README.rst` & `py_auth_micro-0.1.7/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 py_auth_micro
 ================
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://pypi.org/project/black
 
 .. image:: https://app.codacy.com/project/badge/Grade/199fd463ff1a487eb206a2afbfb25168
-    :target: https://www.codacy.com/gh/bad-microservices/py_auth_micro/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=bad-microservices/py_auth_micro&amp;utm_campaign=Badge_Grade
+    :target: https://app.codacy.com/gh/bad-microservices/py_auth_micro/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
 
 .. image:: https://badge.fury.io/py/py-auth-micro.svg
     :target: https://badge.fury.io/py/py-auth-micro
 
 .. image:: https://github.com/bad-microservices/py_auth_micro/actions/workflows/documentation.yaml/badge.svg
    :target: https://github.com/bad-microservices/py_auth_micro/actions?query=workflow:Docs
```

### Comparing `py_auth_micro-0.1.6/py_auth_micro/Config/_appconfig.py` & `py_auth_micro-0.1.7/py_auth_micro/Config/_appconfig.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from dataclasses import dataclass
 
+
 @dataclass
 class AppConfig:
     """A class holding information about the general configuration State.
 
-    Attirbutes:
-        id_token_valid_time (int): How long ID Tokens stay valid (in minutes). Defaults to `1440` (24 hours).
-        access_token_valid_time (int): How long Access Tokens stay valid (in minutes). Defaults to `5`.
-        allow_registration (bool): Can users register themselfs?. Defaults to `False`.
-        auto_activate_accounts (bool): Automatically activate Accounts on creation. Defaults to `True`
-        admin_group (str): Name of the administrator Group. Defaults to `admin`
-        default_vhost (str): Name of the Default VHOST if no VHOST ist given on Login. Defaults to `prod`
-        username_regex (str): Regex to check Usernames with. Defaults to `r"[a-zA-Z-_0-9]{4,30}"`
-        password_regex (str): Regex to check Passwords with. Defaults to `r".{4,}"`
+    Attributes:
+        id_token_valid_time (int): How long ID Tokens stay valid (in minutes). Defaults to :code:`1440` (24 hours).
+        access_token_valid_time (int): How long Access Tokens stay valid (in minutes). Defaults to :code:`5` .
+        allow_registration (bool): Can users register themselfs?. Defaults to :code:`False` .
+        auto_activate_accounts (bool): Automatically activate Accounts on creation. Defaults to :code:`True` .
+        admin_group (str): Name of the administrator Group. Defaults to :code:`admin` .
+        default_vhost (str): Name of the Default VHOST if no VHOST ist given on Login. Defaults to :code:`prod` .
+        username_regex (str): Regex to check Usernames with. Defaults to :code:`r"[a-zA-Z-_0-9]{4,30}"` .
+        password_regex (str): Regex to check Passwords with. Defaults to :code:`r".{4,}"` .
         email_regex (str): Regex to check Emails with. Defaults to a kinda long regex doing basic checks for emails.
     """
-    id_token_valid_time:int = 1440
-    access_token_valid_time:int = 5
+
+    id_token_valid_time: int = 1440
+    access_token_valid_time: int = 5
     allow_registration: bool = False
     auto_activate_accounts: bool = True
     admin_group: str = "admin"
     default_vhost: str = "prod"
-    group_regex:str = r"[a-zA-Z0-9_-]{1,50}"
+    group_regex: str = r"[a-zA-Z0-9_-]{1,50}"
     username_regex: str = r"[a-zA-Z-_0-9]{4,30}"
     password_regex: str = r".{4,}"
     email_regex: str = r"[a-zA-Z0-9.!#$%&'*+\/=?^_`{|}~-]+@[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?(?:\.[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?)"
```

### Comparing `py_auth_micro-0.1.6/py_auth_micro/Config/_dbconfig.py` & `py_auth_micro-0.1.7/py_auth_micro/Config/_dbconfig.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.6/py_auth_micro/Config/_ldapconfig.py` & `py_auth_micro-0.1.7/py_auth_micro/Config/_ldapconfig.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 @dataclass
 class LDAPConfig:
     """a Configuration class storing our AD Related config
 
     Attributes:
         address (str): Server Address.
         base_dn (str): Base DN for Users.
-        group (str, optional): Group that allows the Login itself. Defaults to "allowed_to_login".
-        groups_prefix (str, optional): Prefix of groups that should be added to the User. Defaults to "API_PERM".
-        domain (str, optional): The Domain the user should log into. Defaults to 3306.
-        ca_file (str, optional): Path to the CA File used for ldaps. Defaults to None.
+        group (str, optional): Group that allows the Login itself. Defaults to :code:`"allowed_to_login"`.
+        groups_prefix (str, optional): Prefix of groups that should be added to the User. Defaults to :code:`"API_PERM"`.
+        domain (str, optional): The Domain the user should log into. Defaults to :code:`3306`.
+        ca_file (str, optional): Path to the CA File used for ldaps. Defaults to :code:`None`.
     """
 
     address: str = "ldap://127.0.0.1:389"
     base_dn: str = "ou=User,dc=ad,dc=local"
     group: str = "allowed_to_login"
     groups_prefix: str = "API_PERM"
     domain: str = "ad.local"
```

### Comparing `py_auth_micro-0.1.6/py_auth_micro/Core/_ldap_interactions.py` & `py_auth_micro-0.1.7/py_auth_micro/Core/_ldap_interactions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from dataclasses import dataclass
 try:
     import ldap
 except ImportError:
-    print("cant import python-ldap\nldap connection wont work")
+    print("cant import python-ldap\nldap connection won't work")
 
 from ..Config import LDAPConfig
 
 
 @dataclass
 class LDAPHelper:
     """A class which helps interacting with an LDAP Server
 
     Warning:
-        While instantiating this class it will bin against the LDAP!
+        While instantiating this class it will bind against the LDAP!
 
     Attributes:
         config (LDAPConfig): The Configuration to connect to the LDAP.
         username (str): Name of the User we want to log in with.
         password (str): Password of the user.
     """
```

### Comparing `py_auth_micro-0.1.6/py_auth_micro/LoginHandler/__init__.py` & `py_auth_micro-0.1.7/py_auth_micro/LoginHandler/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 """The :code:`LoginHandler` Package contains classes for different identity Sources.
 
 Currently there are Classes to work with the following identity Sources:
 
     * :code:`LoginLocal` - for a Local Database
     * :code:`LoginLDAP` - for LDAP
-    * :code:`LoginKerberos` - for Kerberos
 
 These are choosen automatically by the :code:`auth_type` field connected to every Users DB Entry.
 The :code:`auth_type` is an :code:`AuthSource`.
 
 """
 import logging
 
 from tortoise.exceptions import DoesNotExist
 from typing import Optional
 
-from ._loginbaseclass import LoginBaseClass
-from ._loginldap import LoginLDAP
-from ._loginkerberos import LoginKerberos
-from ._loginlocal import LoginLocal
-
-from ..Config import LDAPConfig
-from ..Models import User
-
-from ..Core import LDAPHelper, AuthSource
+from py_auth_micro.LoginHandler._loginbaseclass import LoginBaseClass
+from py_auth_micro.LoginHandler._loginldap import LoginLDAP
+from py_auth_micro.LoginHandler._loginlocal import LoginLocal
+
+from py_auth_micro.Config import LDAPConfig
+from py_auth_micro.Models import User
+from py_auth_micro.Core import LDAPHelper, AuthSource
 
 LOGINHANDLER = {
     AuthSource.LDAP: LoginLDAP,
     AuthSource.LOCAL: LoginLocal,
-    AuthSource.KERBEROS: LoginKerberos,
 }
 
 
-
 async def login(
     username: str, password: str, ldap_config: Optional[LDAPConfig] = None
 ) -> User:
     """Function which logs a user in with specified Credentials.
 
     Args:
         username (str): Username of the User
@@ -84,15 +79,17 @@
         logger.info(f"user '{username}' does not exist in DB")
         # try LDAP
         try:
             logger.debug(f"try to auth user '{username}' with ldap")
             helper = LDAPHelper(ldap_config, username, password)
             # if the user can be authenticated with ldap create him in the DB
             if helper.login():
-                logger.debug(f"User '{username}' could auth with the LDAP -> creating DB Entry")
+                logger.debug(
+                    f"User '{username}' could auth with the LDAP -> creating DB Entry"
+                )
                 user = await User.create(
                     username=username,
                     password_hash=None,
                     activated=True,
                     auth_type=AuthSource.LDAP,
                     email=helper.email,
                 )
@@ -101,8 +98,8 @@
             logger.debug(f"user '{username}' could not auth with LDAP")
             raise DoesNotExist
 
         # if the user cant log in with ldap reraise the exc
         raise exc
 
 
-__all__ = ["login", "LoginBaseClass", "LoginLDAP", "LoginLocal", "LoginKerberos"]
+__all__ = ["login", "LoginBaseClass", "LoginLDAP", "LoginLocal"]
```

### Comparing `py_auth_micro-0.1.6/py_auth_micro/LoginHandler/_loginbaseclass.py` & `py_auth_micro-0.1.7/py_auth_micro/LoginHandler/_loginbaseclass.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
 
 
 class LoginBaseClass(ABC):
     """Abstract Baseclass for Authenticating Users
 
-    This Is an abstract baseclass describing all functions needed to be implemented by a generic LoginHandler.
+    This is an abstract baseclass describing all functions needed to be implemented by a generic LoginHandler.
     """
 
     def __init__(self, **kwargs):
         for key, value in kwargs.items():
             if key in self.__annotations__.keys():
                 setattr(self, key, value)
```

### Comparing `py_auth_micro-0.1.6/py_auth_micro/LoginHandler/_loginldap.py` & `py_auth_micro-0.1.7/py_auth_micro/LoginHandler/_loginldap.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.6/py_auth_micro/LoginHandler/_loginlocal.py` & `py_auth_micro-0.1.7/py_auth_micro/LoginHandler/_loginlocal.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.6/py_auth_micro/Models/_token.py` & `py_auth_micro-0.1.7/py_auth_micro/Models/_token.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.6/py_auth_micro/Models/_user.py` & `py_auth_micro-0.1.7/py_auth_micro/Models/_user.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.6/py_auth_micro/WorkFlows/__init__.py` & `py_auth_micro-0.1.7/py_auth_micro/WorkFlows/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """This Package specifies classes which implement the most common workflows.
 
 following workflows are implemented:
 
-    * Sign In
-    * Sign Out
-    * Token Request
-    * Registration
-    * User creation (by Administrators)
-    * User deletion
-    * Group creation (by Administrators)
-    * Group deletion (by Administrators)
-    * Adding User to a Group (by Administrators)
-    * Removing User from a Group (by Administrators)
+    * SessionWorkflow
+       * Sign In
+       * Sign Out
+       * Token Request
+    * UserWorkFlow
+       * Registration
+       * User creation (by Administrators)
+       * User deletion
+    * GroupWorkfFlow
+       * Group creation (by Administrators)
+       * Group deletion (by Administrators)
+       * Adding User to a Group (by Administrators)
+       * Removing User from a Group (by Administrators)
 
 All Function should return Dictionaries which can be easily parsed to JSON
 
 """
 
-from ._userworkflow import UserWorkflow
-from ._sessionworkflow import SessionWorkflow
-from ._groupworkflow import GroupWorkflow
+from py_auth_micro.WorkFlows._userworkflow import UserWorkflow
+from py_auth_micro.WorkFlows._sessionworkflow import SessionWorkflow
+from py_auth_micro.WorkFlows._groupworkflow import GroupWorkflow
+from py_auth_micro.WorkFlows import _misc as misc
 
-__all__ = ["UserWorkflow", "SessionWorkflow","GroupWorkflow"]
+__all__ = ["UserWorkflow", "SessionWorkflow", "GroupWorkflow", "misc"]
```

### Comparing `py_auth_micro-0.1.6/py_auth_micro/WorkFlows/_groupworkflow.py` & `py_auth_micro-0.1.7/py_auth_micro/WorkFlows/_groupworkflow.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.6/py_auth_micro/WorkFlows/_misc.py` & `py_auth_micro-0.1.7/py_auth_micro/WorkFlows/_misc.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.6/py_auth_micro/WorkFlows/_sessionworkflow.py` & `py_auth_micro-0.1.7/py_auth_micro/WorkFlows/_sessionworkflow.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.6/py_auth_micro/WorkFlows/_userworkflow.py` & `py_auth_micro-0.1.7/py_auth_micro/WorkFlows/_userworkflow.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.6/py_auth_micro.egg-info/PKG-INFO` & `py_auth_micro-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py-auth-micro
-Version: 0.1.6
+Name: py_auth_micro
+Version: 0.1.7
 Summary: A wrapper around pyjwt
 Home-page: https://github.com/bad-microservices/py_auth_micro
 Author: Ole Hannemann
 Author-email: cerberus885@gmail.com
 License: MIT
 Keywords: JWT
 Classifier: Programming Language :: Python :: 3.0
@@ -19,15 +19,15 @@
 py_auth_micro
 ================
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://pypi.org/project/black
 
 .. image:: https://app.codacy.com/project/badge/Grade/199fd463ff1a487eb206a2afbfb25168
-    :target: https://www.codacy.com/gh/bad-microservices/py_auth_micro/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=bad-microservices/py_auth_micro&amp;utm_campaign=Badge_Grade
+    :target: https://app.codacy.com/gh/bad-microservices/py_auth_micro/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
 
 .. image:: https://badge.fury.io/py/py-auth-micro.svg
     :target: https://badge.fury.io/py/py-auth-micro
 
 .. image:: https://github.com/bad-microservices/py_auth_micro/actions/workflows/documentation.yaml/badge.svg
    :target: https://github.com/bad-microservices/py_auth_micro/actions?query=workflow:Docs
```

### Comparing `py_auth_micro-0.1.6/py_auth_micro.egg-info/SOURCES.txt` & `py_auth_micro-0.1.7/py_auth_micro.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 py_auth_micro/Config/_ldapconfig.py
 py_auth_micro/Core/__init__.py
 py_auth_micro/Core/_enums.py
 py_auth_micro/Core/_ldap_interactions.py
 py_auth_micro/Exceptions/__init__.py
 py_auth_micro/LoginHandler/__init__.py
 py_auth_micro/LoginHandler/_loginbaseclass.py
-py_auth_micro/LoginHandler/_loginkerberos.py
 py_auth_micro/LoginHandler/_loginldap.py
 py_auth_micro/LoginHandler/_loginlocal.py
 py_auth_micro/Models/__init__.py
 py_auth_micro/Models/_group.py
 py_auth_micro/Models/_token.py
 py_auth_micro/Models/_user.py
 py_auth_micro/WorkFlows/__init__.py
```

### Comparing `py_auth_micro-0.1.6/setup.cfg` & `py_auth_micro-0.1.7/setup.cfg`

 * *Files identical despite different names*

