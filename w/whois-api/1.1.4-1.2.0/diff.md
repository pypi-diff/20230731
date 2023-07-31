# Comparing `tmp/whois-api-1.1.4.tar.gz` & `tmp/whois-api-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whois-api-1.1.4.tar", last modified: Mon Jul 31 10:05:49 2023, max compression
+gzip compressed data, was "whois-api-1.2.0.tar", last modified: Mon Jul 31 11:35:00 2023, max compression
```

## Comparing `whois-api-1.1.4.tar` & `whois-api-1.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:05:49.344200 whois-api-1.1.4/
--rw-r--r--   0 foobar     (501) staff       (20)       81 2021-04-14 07:33:27.000000 whois-api-1.1.4/AUTHORS.rst
--rw-r--r--   0 foobar     (501) staff       (20)      518 2023-07-31 10:04:37.000000 whois-api-1.1.4/CHANGELOG.rst
--rw-r--r--   0 foobar     (501) staff       (20)     1058 2021-04-14 07:33:27.000000 whois-api-1.1.4/LICENSE
--rw-r--r--   0 foobar     (501) staff       (20)      150 2021-04-14 07:33:27.000000 whois-api-1.1.4/MANIFEST.in
--rw-r--r--   0 foobar     (501) staff       (20)     3141 2023-07-31 10:05:49.343944 whois-api-1.1.4/PKG-INFO
--rw-r--r--   0 foobar     (501) staff       (20)     1614 2023-07-31 08:12:01.000000 whois-api-1.1.4/README.rst
--rw-r--r--   0 foobar     (501) staff       (20)       38 2023-07-31 10:05:49.344284 whois-api-1.1.4/setup.cfg
--rw-r--r--   0 foobar     (501) staff       (20)     2062 2023-07-31 10:04:37.000000 whois-api-1.1.4/setup.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:05:49.336211 whois-api-1.1.4/src/
--rw-r--r--   0 foobar     (501) staff       (20)       23 2021-04-14 08:34:58.000000 whois-api-1.1.4/src/__init__.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:05:49.338226 whois-api-1.1.4/src/whois_api.egg-info/
--rw-r--r--   0 foobar     (501) staff       (20)     3141 2023-07-31 10:05:49.000000 whois-api-1.1.4/src/whois_api.egg-info/PKG-INFO
--rw-r--r--   0 foobar     (501) staff       (20)      634 2023-07-31 10:05:49.000000 whois-api-1.1.4/src/whois_api.egg-info/SOURCES.txt
--rw-r--r--   0 foobar     (501) staff       (20)        1 2023-07-31 10:05:49.000000 whois-api-1.1.4/src/whois_api.egg-info/dependency_links.txt
--rw-r--r--   0 foobar     (501) staff       (20)        1 2023-07-31 10:05:49.000000 whois-api-1.1.4/src/whois_api.egg-info/not-zip-safe
--rw-r--r--   0 foobar     (501) staff       (20)       20 2023-07-31 10:05:49.000000 whois-api-1.1.4/src/whois_api.egg-info/requires.txt
--rw-r--r--   0 foobar     (501) staff       (20)       18 2023-07-31 10:05:49.000000 whois-api-1.1.4/src/whois_api.egg-info/top_level.txt
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:05:49.339084 whois-api-1.1.4/src/whoisapi/
--rw-r--r--   0 foobar     (501) staff       (20)      712 2021-11-19 14:11:58.000000 whois-api-1.1.4/src/whoisapi/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)     3177 2021-11-19 14:11:58.000000 whois-api-1.1.4/src/whoisapi/client.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:05:49.339821 whois-api-1.1.4/src/whoisapi/exceptions/
--rw-r--r--   0 foobar     (501) staff       (20)      312 2021-11-19 14:11:58.000000 whois-api-1.1.4/src/whoisapi/exceptions/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)     1186 2021-11-19 14:11:58.000000 whois-api-1.1.4/src/whoisapi/exceptions/error.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:05:49.341133 whois-api-1.1.4/src/whoisapi/models/
--rw-r--r--   0 foobar     (501) staff       (20)      262 2021-04-14 07:33:27.000000 whois-api-1.1.4/src/whoisapi/models/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)      600 2021-04-14 07:33:27.000000 whois-api-1.1.4/src/whoisapi/models/base.py
--rw-r--r--   0 foobar     (501) staff       (20)     5618 2021-11-19 14:11:58.000000 whois-api-1.1.4/src/whoisapi/models/request.py
--rw-r--r--   0 foobar     (501) staff       (20)    12929 2023-07-31 09:53:06.000000 whois-api-1.1.4/src/whoisapi/models/response.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:05:49.342552 whois-api-1.1.4/src/whoisapi/net/
--rw-r--r--   0 foobar     (501) staff       (20)       59 2021-04-14 07:33:27.000000 whois-api-1.1.4/src/whoisapi/net/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)     3369 2021-04-14 07:33:27.000000 whois-api-1.1.4/src/whoisapi/net/http.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:05:49.343463 whois-api-1.1.4/tests/
--rw-r--r--   0 foobar     (501) staff       (20)        0 2021-04-14 07:33:27.000000 whois-api-1.1.4/tests/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)     2012 2021-04-14 10:02:07.000000 whois-api-1.1.4/tests/client_test.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 11:35:00.833040 whois-api-1.2.0/
+-rw-r--r--   0 foobar     (501) staff       (20)       81 2021-04-14 07:33:27.000000 whois-api-1.2.0/AUTHORS.rst
+-rw-r--r--   0 foobar     (501) staff       (20)      581 2023-07-31 11:33:13.000000 whois-api-1.2.0/CHANGELOG.rst
+-rw-r--r--   0 foobar     (501) staff       (20)     1058 2021-04-14 07:33:27.000000 whois-api-1.2.0/LICENSE
+-rw-r--r--   0 foobar     (501) staff       (20)      150 2021-04-14 07:33:27.000000 whois-api-1.2.0/MANIFEST.in
+-rw-r--r--   0 foobar     (501) staff       (20)     3204 2023-07-31 11:35:00.832268 whois-api-1.2.0/PKG-INFO
+-rw-r--r--   0 foobar     (501) staff       (20)     1614 2023-07-31 08:12:01.000000 whois-api-1.2.0/README.rst
+-rw-r--r--   0 foobar     (501) staff       (20)       38 2023-07-31 11:35:00.833463 whois-api-1.2.0/setup.cfg
+-rw-r--r--   0 foobar     (501) staff       (20)     2062 2023-07-31 11:31:22.000000 whois-api-1.2.0/setup.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 11:35:00.822259 whois-api-1.2.0/src/
+-rw-r--r--   0 foobar     (501) staff       (20)       23 2021-04-14 08:34:58.000000 whois-api-1.2.0/src/__init__.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 11:35:00.824789 whois-api-1.2.0/src/whois_api.egg-info/
+-rw-r--r--   0 foobar     (501) staff       (20)     3204 2023-07-31 11:35:00.000000 whois-api-1.2.0/src/whois_api.egg-info/PKG-INFO
+-rw-r--r--   0 foobar     (501) staff       (20)      634 2023-07-31 11:35:00.000000 whois-api-1.2.0/src/whois_api.egg-info/SOURCES.txt
+-rw-r--r--   0 foobar     (501) staff       (20)        1 2023-07-31 11:35:00.000000 whois-api-1.2.0/src/whois_api.egg-info/dependency_links.txt
+-rw-r--r--   0 foobar     (501) staff       (20)        1 2023-07-31 11:35:00.000000 whois-api-1.2.0/src/whois_api.egg-info/not-zip-safe
+-rw-r--r--   0 foobar     (501) staff       (20)       20 2023-07-31 11:35:00.000000 whois-api-1.2.0/src/whois_api.egg-info/requires.txt
+-rw-r--r--   0 foobar     (501) staff       (20)       18 2023-07-31 11:35:00.000000 whois-api-1.2.0/src/whois_api.egg-info/top_level.txt
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 11:35:00.825517 whois-api-1.2.0/src/whoisapi/
+-rw-r--r--   0 foobar     (501) staff       (20)      712 2021-11-19 14:11:58.000000 whois-api-1.2.0/src/whoisapi/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)     3177 2021-11-19 14:11:58.000000 whois-api-1.2.0/src/whoisapi/client.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 11:35:00.826426 whois-api-1.2.0/src/whoisapi/exceptions/
+-rw-r--r--   0 foobar     (501) staff       (20)      312 2021-11-19 14:11:58.000000 whois-api-1.2.0/src/whoisapi/exceptions/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)     1186 2021-11-19 14:11:58.000000 whois-api-1.2.0/src/whoisapi/exceptions/error.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 11:35:00.828001 whois-api-1.2.0/src/whoisapi/models/
+-rw-r--r--   0 foobar     (501) staff       (20)      262 2021-04-14 07:33:27.000000 whois-api-1.2.0/src/whoisapi/models/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)      600 2021-04-14 07:33:27.000000 whois-api-1.2.0/src/whoisapi/models/base.py
+-rw-r--r--   0 foobar     (501) staff       (20)     5618 2021-11-19 14:11:58.000000 whois-api-1.2.0/src/whoisapi/models/request.py
+-rw-r--r--   0 foobar     (501) staff       (20)    12931 2023-07-31 11:02:25.000000 whois-api-1.2.0/src/whoisapi/models/response.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 11:35:00.830130 whois-api-1.2.0/src/whoisapi/net/
+-rw-r--r--   0 foobar     (501) staff       (20)       59 2021-04-14 07:33:27.000000 whois-api-1.2.0/src/whoisapi/net/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)     3369 2021-04-14 07:33:27.000000 whois-api-1.2.0/src/whoisapi/net/http.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 11:35:00.831328 whois-api-1.2.0/tests/
+-rw-r--r--   0 foobar     (501) staff       (20)        0 2021-04-14 07:33:27.000000 whois-api-1.2.0/tests/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)     2012 2021-04-14 10:02:07.000000 whois-api-1.2.0/tests/client_test.py
```

### Comparing `whois-api-1.1.4/LICENSE` & `whois-api-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.4/PKG-INFO` & `whois-api-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whois-api
-Version: 1.1.4
+Version: 1.2.0
 Summary: Python client library for Whois API.
 Home-page: https://github.com/whois-api-llc/whois-api-py
 Author: WHOIS API, Inc
 Author-email: support@whoisxmlapi.com
 License: MIT
 Keywords: whois,api,whoisxmlapi
 Classifier: Development Status :: 5 - Production/Stable
@@ -97,14 +97,19 @@
     client.parameters.output_format = 'xml'
     print(client.raw_data('whoisxmlapi.com'))
 
 
 Changelog
 =========
 
+1.2.0 (2023-07-31)
+------------------
+
+* Fix datetime parsing
+
 1.1.4 (2023-07-31)
 ------------------
 
 * Fix datetime parsing
 * Add postal_code_str field
 
 1.1.3 (2023-07-31)
```

### Comparing `whois-api-1.1.4/README.rst` & `whois-api-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.4/setup.py` & `whois-api-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         join(dirname(__file__), *names),
         encoding=kwargs.get('encoding', 'utf8')
     ).read()
 
 
 setup(
     name='whois-api',
-    version='1.1.4',
+    version='1.2.0',
     python_requires='~=3.7',
     license='MIT',
     description='Python client library for Whois API.',
     long_description='%s\n%s' % (
         re.compile('^.. start-badges.*^.. end-badges', re.M | re.S).sub('', read('README.rst')),
         re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst'))
     ),
```

### Comparing `whois-api-1.1.4/src/whois_api.egg-info/PKG-INFO` & `whois-api-1.2.0/src/whois_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whois-api
-Version: 1.1.4
+Version: 1.2.0
 Summary: Python client library for Whois API.
 Home-page: https://github.com/whois-api-llc/whois-api-py
 Author: WHOIS API, Inc
 Author-email: support@whoisxmlapi.com
 License: MIT
 Keywords: whois,api,whoisxmlapi
 Classifier: Development Status :: 5 - Production/Stable
@@ -97,14 +97,19 @@
     client.parameters.output_format = 'xml'
     print(client.raw_data('whoisxmlapi.com'))
 
 
 Changelog
 =========
 
+1.2.0 (2023-07-31)
+------------------
+
+* Fix datetime parsing
+
 1.1.4 (2023-07-31)
 ------------------
 
 * Fix datetime parsing
 * Add postal_code_str field
 
 1.1.3 (2023-07-31)
```

### Comparing `whois-api-1.1.4/src/whois_api.egg-info/SOURCES.txt` & `whois-api-1.2.0/src/whois_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.4/src/whoisapi/__init__.py` & `whois-api-1.2.0/src/whoisapi/__init__.py`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.4/src/whoisapi/client.py` & `whois-api-1.2.0/src/whoisapi/client.py`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.4/src/whoisapi/exceptions/error.py` & `whois-api-1.2.0/src/whoisapi/exceptions/error.py`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.4/src/whoisapi/models/base.py` & `whois-api-1.2.0/src/whoisapi/models/base.py`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.4/src/whoisapi/models/request.py` & `whois-api-1.2.0/src/whoisapi/models/request.py`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.4/src/whoisapi/models/response.py` & `whois-api-1.2.0/src/whoisapi/models/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         m = re_milliseconds_and_timezone_offset.search(dt)
         m2 = re_timezone_offset.search(dt)
         m3 = re_milliseconds_and_timezone_name.search(dt)
         m4 = re_coordinated_utc.search(dt)
         try:
             if m is not None:
                 return datetime.datetime.strptime(
-                    re_milliseconds_and_timezone_offset.sub(r'\1\2\3\5'),
+                    re_milliseconds_and_timezone_offset.sub(r'\2\3\5', dt),
                     "%Y-%m-%dT%H:%M:%S%z")
             if m2 is not None:
                 return datetime.datetime.strptime(
                     re_timezone_offset.sub(r'\1\2\4', dt),
                     "%Y-%m-%dT%H:%M:%S%z")
             if m3 is not None:
                 return datetime.datetime.strptime(
```

### Comparing `whois-api-1.1.4/src/whoisapi/net/http.py` & `whois-api-1.2.0/src/whoisapi/net/http.py`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.4/tests/client_test.py` & `whois-api-1.2.0/tests/client_test.py`

 * *Files identical despite different names*

