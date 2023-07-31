# Comparing `tmp/whois-api-1.1.3.tar.gz` & `tmp/whois-api-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whois-api-1.1.3.tar", last modified: Mon Jul 31 09:35:05 2023, max compression
+gzip compressed data, was "whois-api-1.1.4.tar", last modified: Mon Jul 31 10:05:49 2023, max compression
```

## Comparing `whois-api-1.1.3.tar` & `whois-api-1.1.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 09:35:05.031524 whois-api-1.1.3/
--rw-r--r--   0 foobar     (501) staff       (20)       81 2021-04-14 07:33:27.000000 whois-api-1.1.3/AUTHORS.rst
--rw-r--r--   0 foobar     (501) staff       (20)      427 2023-07-31 08:35:10.000000 whois-api-1.1.3/CHANGELOG.rst
--rw-r--r--   0 foobar     (501) staff       (20)     1058 2021-04-14 07:33:27.000000 whois-api-1.1.3/LICENSE
--rw-r--r--   0 foobar     (501) staff       (20)      150 2021-04-14 07:33:27.000000 whois-api-1.1.3/MANIFEST.in
--rw-r--r--   0 foobar     (501) staff       (20)     3050 2023-07-31 09:35:05.031042 whois-api-1.1.3/PKG-INFO
--rw-r--r--   0 foobar     (501) staff       (20)     1614 2023-07-31 08:12:01.000000 whois-api-1.1.3/README.rst
--rw-r--r--   0 foobar     (501) staff       (20)       38 2023-07-31 09:35:05.031715 whois-api-1.1.3/setup.cfg
--rw-r--r--   0 foobar     (501) staff       (20)     2062 2023-07-31 08:35:10.000000 whois-api-1.1.3/setup.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 09:35:05.020141 whois-api-1.1.3/src/
--rw-r--r--   0 foobar     (501) staff       (20)       23 2021-04-14 08:34:58.000000 whois-api-1.1.3/src/__init__.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 09:35:05.023158 whois-api-1.1.3/src/whois_api.egg-info/
--rw-r--r--   0 foobar     (501) staff       (20)     3050 2023-07-31 09:35:05.000000 whois-api-1.1.3/src/whois_api.egg-info/PKG-INFO
--rw-r--r--   0 foobar     (501) staff       (20)      634 2023-07-31 09:35:05.000000 whois-api-1.1.3/src/whois_api.egg-info/SOURCES.txt
--rw-r--r--   0 foobar     (501) staff       (20)        1 2023-07-31 09:35:05.000000 whois-api-1.1.3/src/whois_api.egg-info/dependency_links.txt
--rw-r--r--   0 foobar     (501) staff       (20)        1 2023-07-31 09:33:16.000000 whois-api-1.1.3/src/whois_api.egg-info/not-zip-safe
--rw-r--r--   0 foobar     (501) staff       (20)       20 2023-07-31 09:35:05.000000 whois-api-1.1.3/src/whois_api.egg-info/requires.txt
--rw-r--r--   0 foobar     (501) staff       (20)       18 2023-07-31 09:35:05.000000 whois-api-1.1.3/src/whois_api.egg-info/top_level.txt
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 09:35:05.024061 whois-api-1.1.3/src/whoisapi/
--rw-r--r--   0 foobar     (501) staff       (20)      712 2021-11-19 14:11:58.000000 whois-api-1.1.3/src/whoisapi/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)     3177 2021-11-19 14:11:58.000000 whois-api-1.1.3/src/whoisapi/client.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 09:35:05.024988 whois-api-1.1.3/src/whoisapi/exceptions/
--rw-r--r--   0 foobar     (501) staff       (20)      312 2021-11-19 14:11:58.000000 whois-api-1.1.3/src/whoisapi/exceptions/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)     1186 2021-11-19 14:11:58.000000 whois-api-1.1.3/src/whoisapi/exceptions/error.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 09:35:05.027477 whois-api-1.1.3/src/whoisapi/models/
--rw-r--r--   0 foobar     (501) staff       (20)      262 2021-04-14 07:33:27.000000 whois-api-1.1.3/src/whoisapi/models/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)      600 2021-04-14 07:33:27.000000 whois-api-1.1.3/src/whoisapi/models/base.py
--rw-r--r--   0 foobar     (501) staff       (20)     5618 2021-11-19 14:11:58.000000 whois-api-1.1.3/src/whoisapi/models/request.py
--rw-r--r--   0 foobar     (501) staff       (20)    12429 2023-07-31 08:36:47.000000 whois-api-1.1.3/src/whoisapi/models/response.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 09:35:05.029199 whois-api-1.1.3/src/whoisapi/net/
--rw-r--r--   0 foobar     (501) staff       (20)       59 2021-04-14 07:33:27.000000 whois-api-1.1.3/src/whoisapi/net/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)     3369 2021-04-14 07:33:27.000000 whois-api-1.1.3/src/whoisapi/net/http.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 09:35:05.030258 whois-api-1.1.3/tests/
--rw-r--r--   0 foobar     (501) staff       (20)        0 2021-04-14 07:33:27.000000 whois-api-1.1.3/tests/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)     2012 2021-04-14 10:02:07.000000 whois-api-1.1.3/tests/client_test.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:05:49.344200 whois-api-1.1.4/
+-rw-r--r--   0 foobar     (501) staff       (20)       81 2021-04-14 07:33:27.000000 whois-api-1.1.4/AUTHORS.rst
+-rw-r--r--   0 foobar     (501) staff       (20)      518 2023-07-31 10:04:37.000000 whois-api-1.1.4/CHANGELOG.rst
+-rw-r--r--   0 foobar     (501) staff       (20)     1058 2021-04-14 07:33:27.000000 whois-api-1.1.4/LICENSE
+-rw-r--r--   0 foobar     (501) staff       (20)      150 2021-04-14 07:33:27.000000 whois-api-1.1.4/MANIFEST.in
+-rw-r--r--   0 foobar     (501) staff       (20)     3141 2023-07-31 10:05:49.343944 whois-api-1.1.4/PKG-INFO
+-rw-r--r--   0 foobar     (501) staff       (20)     1614 2023-07-31 08:12:01.000000 whois-api-1.1.4/README.rst
+-rw-r--r--   0 foobar     (501) staff       (20)       38 2023-07-31 10:05:49.344284 whois-api-1.1.4/setup.cfg
+-rw-r--r--   0 foobar     (501) staff       (20)     2062 2023-07-31 10:04:37.000000 whois-api-1.1.4/setup.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:05:49.336211 whois-api-1.1.4/src/
+-rw-r--r--   0 foobar     (501) staff       (20)       23 2021-04-14 08:34:58.000000 whois-api-1.1.4/src/__init__.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:05:49.338226 whois-api-1.1.4/src/whois_api.egg-info/
+-rw-r--r--   0 foobar     (501) staff       (20)     3141 2023-07-31 10:05:49.000000 whois-api-1.1.4/src/whois_api.egg-info/PKG-INFO
+-rw-r--r--   0 foobar     (501) staff       (20)      634 2023-07-31 10:05:49.000000 whois-api-1.1.4/src/whois_api.egg-info/SOURCES.txt
+-rw-r--r--   0 foobar     (501) staff       (20)        1 2023-07-31 10:05:49.000000 whois-api-1.1.4/src/whois_api.egg-info/dependency_links.txt
+-rw-r--r--   0 foobar     (501) staff       (20)        1 2023-07-31 10:05:49.000000 whois-api-1.1.4/src/whois_api.egg-info/not-zip-safe
+-rw-r--r--   0 foobar     (501) staff       (20)       20 2023-07-31 10:05:49.000000 whois-api-1.1.4/src/whois_api.egg-info/requires.txt
+-rw-r--r--   0 foobar     (501) staff       (20)       18 2023-07-31 10:05:49.000000 whois-api-1.1.4/src/whois_api.egg-info/top_level.txt
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:05:49.339084 whois-api-1.1.4/src/whoisapi/
+-rw-r--r--   0 foobar     (501) staff       (20)      712 2021-11-19 14:11:58.000000 whois-api-1.1.4/src/whoisapi/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)     3177 2021-11-19 14:11:58.000000 whois-api-1.1.4/src/whoisapi/client.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:05:49.339821 whois-api-1.1.4/src/whoisapi/exceptions/
+-rw-r--r--   0 foobar     (501) staff       (20)      312 2021-11-19 14:11:58.000000 whois-api-1.1.4/src/whoisapi/exceptions/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)     1186 2021-11-19 14:11:58.000000 whois-api-1.1.4/src/whoisapi/exceptions/error.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:05:49.341133 whois-api-1.1.4/src/whoisapi/models/
+-rw-r--r--   0 foobar     (501) staff       (20)      262 2021-04-14 07:33:27.000000 whois-api-1.1.4/src/whoisapi/models/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)      600 2021-04-14 07:33:27.000000 whois-api-1.1.4/src/whoisapi/models/base.py
+-rw-r--r--   0 foobar     (501) staff       (20)     5618 2021-11-19 14:11:58.000000 whois-api-1.1.4/src/whoisapi/models/request.py
+-rw-r--r--   0 foobar     (501) staff       (20)    12929 2023-07-31 09:53:06.000000 whois-api-1.1.4/src/whoisapi/models/response.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:05:49.342552 whois-api-1.1.4/src/whoisapi/net/
+-rw-r--r--   0 foobar     (501) staff       (20)       59 2021-04-14 07:33:27.000000 whois-api-1.1.4/src/whoisapi/net/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)     3369 2021-04-14 07:33:27.000000 whois-api-1.1.4/src/whoisapi/net/http.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:05:49.343463 whois-api-1.1.4/tests/
+-rw-r--r--   0 foobar     (501) staff       (20)        0 2021-04-14 07:33:27.000000 whois-api-1.1.4/tests/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)     2012 2021-04-14 10:02:07.000000 whois-api-1.1.4/tests/client_test.py
```

### Comparing `whois-api-1.1.3/LICENSE` & `whois-api-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.3/PKG-INFO` & `whois-api-1.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whois-api
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python client library for Whois API.
 Home-page: https://github.com/whois-api-llc/whois-api-py
 Author: WHOIS API, Inc
 Author-email: support@whoisxmlapi.com
 License: MIT
 Keywords: whois,api,whoisxmlapi
 Classifier: Development Status :: 5 - Production/Stable
@@ -97,14 +97,20 @@
     client.parameters.output_format = 'xml'
     print(client.raw_data('whoisxmlapi.com'))
 
 
 Changelog
 =========
 
+1.1.4 (2023-07-31)
+------------------
+
+* Fix datetime parsing
+* Add postal_code_str field
+
 1.1.3 (2023-07-31)
 ------------------
 
 * Bump requests
 * Drop Python 3.6 support
 
 1.1.2 (2022-11-08)
```

### Comparing `whois-api-1.1.3/README.rst` & `whois-api-1.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.3/setup.py` & `whois-api-1.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         join(dirname(__file__), *names),
         encoding=kwargs.get('encoding', 'utf8')
     ).read()
 
 
 setup(
     name='whois-api',
-    version='1.1.3',
+    version='1.1.4',
     python_requires='~=3.7',
     license='MIT',
     description='Python client library for Whois API.',
     long_description='%s\n%s' % (
         re.compile('^.. start-badges.*^.. end-badges', re.M | re.S).sub('', read('README.rst')),
         re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst'))
     ),
```

### Comparing `whois-api-1.1.3/src/whois_api.egg-info/PKG-INFO` & `whois-api-1.1.4/src/whois_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whois-api
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python client library for Whois API.
 Home-page: https://github.com/whois-api-llc/whois-api-py
 Author: WHOIS API, Inc
 Author-email: support@whoisxmlapi.com
 License: MIT
 Keywords: whois,api,whoisxmlapi
 Classifier: Development Status :: 5 - Production/Stable
@@ -97,14 +97,20 @@
     client.parameters.output_format = 'xml'
     print(client.raw_data('whoisxmlapi.com'))
 
 
 Changelog
 =========
 
+1.1.4 (2023-07-31)
+------------------
+
+* Fix datetime parsing
+* Add postal_code_str field
+
 1.1.3 (2023-07-31)
 ------------------
 
 * Bump requests
 * Drop Python 3.6 support
 
 1.1.2 (2022-11-08)
```

### Comparing `whois-api-1.1.3/src/whois_api.egg-info/SOURCES.txt` & `whois-api-1.1.4/src/whois_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.3/src/whoisapi/__init__.py` & `whois-api-1.1.4/src/whoisapi/__init__.py`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.3/src/whoisapi/client.py` & `whois-api-1.1.4/src/whoisapi/client.py`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.3/src/whoisapi/exceptions/error.py` & `whois-api-1.1.4/src/whoisapi/exceptions/error.py`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.3/src/whoisapi/models/base.py` & `whois-api-1.1.4/src/whoisapi/models/base.py`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.3/src/whoisapi/models/request.py` & `whois-api-1.1.4/src/whoisapi/models/request.py`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.3/src/whoisapi/models/response.py` & `whois-api-1.1.4/src/whoisapi/models/response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import datetime
 import copy
 import re
 import logging
 from .base import BaseModel
 
-
 _logger = logging.getLogger('whois-api-client-models')
 
+re_milliseconds_and_timezone_offset = re.compile(r'(\.\d\d\d)?([-+])(\d\d)(:)?(\d\d)$')
 re_timezone_offset = re.compile(r'([-+])(\d\d)(:)?(\d\d)$')
 re_coordinated_utc = re.compile(r'(T\d\d:\d\d:\d\dZ)$')
 re_milliseconds_and_timezone_name = re.compile(
     r'(\.\d\d\d)?\s+([a-z]{3,4})$', re.IGNORECASE)
 
 
 def _string_value(values: dict, key: str) -> str:
@@ -21,47 +21,52 @@
 
 def _int_value(values: dict, key: str) -> int:
     if key in values:
         try:
             return int(values[key])
         except (ValueError, Exception) as error:
             _logger.error(
-            "Couldn't parse the int ({}: {}). Error occurred: {}".format(
-                key,
-                values[key],
-                error.__str__()
+                "Couldn't parse the int ({}: {}). Error occurred: {}".format(
+                    key,
+                    values[key],
+                    error.__str__()
+                )
             )
-        )
     return 0
 
 
 def _list_value(values: dict, key: str) -> list:
     if key in values and type(values[key]) is list:
         return copy.deepcopy(values[key])
     return []
 
 
 def _datetime_value(values: dict, key: str) -> datetime.datetime or None:
     if key in values:
         if values[key] is None:
             return None
         dt = str(values[key])
-        m = re_timezone_offset.search(dt)
-        m2 = re_milliseconds_and_timezone_name.search(dt)
-        m3 = re_coordinated_utc.search(dt)
+        m = re_milliseconds_and_timezone_offset.search(dt)
+        m2 = re_timezone_offset.search(dt)
+        m3 = re_milliseconds_and_timezone_name.search(dt)
+        m4 = re_coordinated_utc.search(dt)
         try:
             if m is not None:
                 return datetime.datetime.strptime(
-                    re_timezone_offset.sub(r'\1\2\4', dt),
+                    re_milliseconds_and_timezone_offset.sub(r'\1\2\3\5'),
                     "%Y-%m-%dT%H:%M:%S%z")
             if m2 is not None:
                 return datetime.datetime.strptime(
+                    re_timezone_offset.sub(r'\1\2\4', dt),
+                    "%Y-%m-%dT%H:%M:%S%z")
+            if m3 is not None:
+                return datetime.datetime.strptime(
                     re_milliseconds_and_timezone_name.sub(r' \2', dt),
                     "%Y-%m-%d %H:%M:%S %Z")
-            if m3 is not None:
+            if m4 is not None:
                 return datetime.datetime.strptime(dt, '%Y-%m-%dT%H:%M:%SZ')
         except (ValueError, Exception) as error:
             _logger.error(
                 "Couldn't parse the date ({}). Error occurred: {}".format(
                     dt,
                     error.__str__()
                 )
@@ -118,14 +123,15 @@
     street1: str
     street2: str
     street3: str
     street4: str
     city: str
     state: str
     postal_code: int
+    postal_code_str: str
     country: str
     country_code: str
     email: str
     telephone: str
     telephone_ext: str
     fax: str
     fax_ext: str
@@ -138,14 +144,15 @@
         self.street1 = ''
         self.street2 = ''
         self.street3 = ''
         self.street4 = ''
         self.city = ''
         self.state = ''
         self.postal_code = 0
+        self.postal_code_str = ''
         self.country = ''
         self.country_code = ''
         self.email = ''
         self.telephone = ''
         self.telephone_ext = ''
         self.fax = ''
         self.fax_ext = ''
@@ -156,14 +163,15 @@
             self.street1 = _string_value(values, 'street1')
             self.street2 = _string_value(values, 'street2')
             self.street3 = _string_value(values, 'street3')
             self.street4 = _string_value(values, 'street4')
             self.city = _string_value(values, 'city')
             self.state = _string_value(values, 'state')
             self.postal_code = _int_value(values, 'postalCode')
+            self.postal_code_str = _string_value(values, 'postalCode')
             self.country = _string_value(values, 'country')
             self.country_code = _string_value(values, 'countryCode')
             self.email = _string_value(values, 'email')
             self.telephone = _string_value(values, 'telephone')
             self.telephone_ext = _string_value(values, 'telephoneExt')
             self.fax = _string_value(values, 'fax')
             self.fax_ext = _string_value(values, 'faxExt')
```

### Comparing `whois-api-1.1.3/src/whoisapi/net/http.py` & `whois-api-1.1.4/src/whoisapi/net/http.py`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.3/tests/client_test.py` & `whois-api-1.1.4/tests/client_test.py`

 * *Files identical despite different names*

