# Comparing `tmp/py3simplesoap-0.10.18.tar.gz` & `tmp/py3simplesoap-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py3simplesoap-0.10.18.tar", last modified: Thu Nov 19 05:11:38 2020, max compression
+gzip compressed data, was "py3simplesoap-0.2.tar", last modified: Mon Jul 31 03:35:00 2023, max compression
```

## Comparing `py3simplesoap-0.10.18.tar` & `py3simplesoap-0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 rey       (1000) rey       (1000)        0 2020-11-19 05:11:38.000000 py3simplesoap-0.10.18/
--rw-r--r--   0 rey       (1000) rey       (1000)      707 2020-11-19 05:11:38.000000 py3simplesoap-0.10.18/PKG-INFO
--rw-r--r--   0 rey       (1000) rey       (1000)     3501 2020-11-19 05:11:28.000000 py3simplesoap-0.10.18/README.md
-drwxr-xr-x   0 rey       (1000) rey       (1000)        0 2020-11-19 05:11:38.000000 py3simplesoap-0.10.18/py3simplesoap/
--rw-r--r--   0 rey       (1000) rey       (1000)      151 2020-11-19 05:11:28.000000 py3simplesoap-0.10.18/py3simplesoap/__init__.py
--rw-r--r--   0 rey       (1000) rey       (1000)    38408 2020-11-19 05:08:41.000000 py3simplesoap-0.10.18/py3simplesoap/client.py
--rw-r--r--   0 rey       (1000) rey       (1000)    22994 2020-11-19 05:11:28.000000 py3simplesoap-0.10.18/py3simplesoap/server.py
--rw-r--r--   0 rey       (1000) rey       (1000)    24757 2020-11-19 05:09:03.000000 py3simplesoap-0.10.18/py3simplesoap/simplexml.py
--rw-r--r--   0 rey       (1000) rey       (1000)    12141 2020-11-19 05:09:03.000000 py3simplesoap-0.10.18/py3simplesoap/transport.py
-drwxr-xr-x   0 rey       (1000) rey       (1000)        0 2020-11-19 05:11:38.000000 py3simplesoap-0.10.18/py3simplesoap.egg-info/
--rw-r--r--   0 rey       (1000) rey       (1000)      707 2020-11-19 05:11:38.000000 py3simplesoap-0.10.18/py3simplesoap.egg-info/PKG-INFO
--rw-r--r--   0 rey       (1000) rey       (1000)      294 2020-11-19 05:11:38.000000 py3simplesoap-0.10.18/py3simplesoap.egg-info/SOURCES.txt
--rw-r--r--   0 rey       (1000) rey       (1000)        1 2020-11-19 05:11:38.000000 py3simplesoap-0.10.18/py3simplesoap.egg-info/dependency_links.txt
--rw-r--r--   0 rey       (1000) rey       (1000)       14 2020-11-19 05:11:38.000000 py3simplesoap-0.10.18/py3simplesoap.egg-info/top_level.txt
--rw-r--r--   0 rey       (1000) rey       (1000)       38 2020-11-19 05:11:38.000000 py3simplesoap-0.10.18/setup.cfg
--rw-r--r--   0 rey       (1000) rey       (1000)      849 2020-11-19 05:11:28.000000 py3simplesoap-0.10.18/setup.py
+drwxr-xr-x   0 far        (501) staff       (20)        0 2023-07-31 03:35:00.212236 py3simplesoap-0.2/
+-rw-r--r--   0 far        (501) staff       (20)      670 2023-07-31 03:35:00.212312 py3simplesoap-0.2/PKG-INFO
+-rw-r--r--   0 far        (501) staff       (20)     4074 2023-07-31 03:30:58.000000 py3simplesoap-0.2/README.md
+drwxr-xr-x   0 far        (501) staff       (20)        0 2023-07-31 03:35:00.210804 py3simplesoap-0.2/py3simplesoap/
+-rw-r--r--   0 far        (501) staff       (20)      150 2023-07-31 03:30:58.000000 py3simplesoap-0.2/py3simplesoap/__init__.py
+-rw-r--r--   0 far        (501) staff       (20)    38671 2023-07-31 03:30:58.000000 py3simplesoap-0.2/py3simplesoap/client.py
+-rw-r--r--   0 far        (501) staff       (20)    28906 2023-07-31 03:30:58.000000 py3simplesoap-0.2/py3simplesoap/helpers.py
+-rw-r--r--   0 far        (501) staff       (20)    22991 2023-07-31 03:30:58.000000 py3simplesoap-0.2/py3simplesoap/server.py
+-rw-r--r--   0 far        (501) staff       (20)    24162 2023-07-31 03:30:58.000000 py3simplesoap-0.2/py3simplesoap/simplexml.py
+-rw-r--r--   0 far        (501) staff       (20)    12080 2023-07-31 03:30:58.000000 py3simplesoap-0.2/py3simplesoap/transport.py
+drwxr-xr-x   0 far        (501) staff       (20)        0 2023-07-31 03:35:00.212045 py3simplesoap-0.2/py3simplesoap.egg-info/
+-rw-r--r--   0 far        (501) staff       (20)      670 2023-07-31 03:35:00.000000 py3simplesoap-0.2/py3simplesoap.egg-info/PKG-INFO
+-rw-r--r--   0 far        (501) staff       (20)      329 2023-07-31 03:35:00.000000 py3simplesoap-0.2/py3simplesoap.egg-info/SOURCES.txt
+-rw-r--r--   0 far        (501) staff       (20)        1 2023-07-31 03:35:00.000000 py3simplesoap-0.2/py3simplesoap.egg-info/dependency_links.txt
+-rw-r--r--   0 far        (501) staff       (20)       14 2023-07-31 03:35:00.000000 py3simplesoap-0.2/py3simplesoap.egg-info/top_level.txt
+-rw-r--r--   0 far        (501) staff       (20)      108 2023-07-31 03:35:00.212600 py3simplesoap-0.2/setup.cfg
+-rw-r--r--   0 far        (501) staff       (20)      876 2023-07-31 03:34:48.000000 py3simplesoap-0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `py3simplesoap-0.10.18/README.md` & `py3simplesoap-0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,23 @@
-py3simplesoap / soap2py
+PySimpleSOAP / soap2py
 ======================
 
 Python simple and lightweight SOAP library for client and server webservices interfaces, aimed to be as small and easy as possible, supporting most common functionality.
 Initially it was inspired by [PHP Soap Extension](http://php.net/manual/en/book.soap.php) (mimicking its functionality, simplicity and ease of use), with many advanced features added.
 
-This is a **Stable Branch** ("stable_py3k")
-mainly to be used with [https://github.com/reingart/pyafipws/tree/py3k]() under
-Python 3
+This is a **Stable Branch** ("long-term-support" / bug-fixes for 1.08.x series)
+mainly to be used with [PyAfipWs](https://github.com/reingart/pyafipws) under
+Python 2.7
+
+For new developments, please use **Master Branch** (1.16 version), that has
+newer features and supports Python 3
+
+Sadly, in the migration from GoogleCode, there was some issue with hg/git and
+now these two branches have entirely different commit histories.
+A manual merge is expected to reunify the codebase soon.
 
 Changelog
 ---------
 
 Last features (2014-2017):
 
  * Add ns prefix for new server type '.net' (in clients)
@@ -42,22 +49,36 @@
 
 Client initially developed for AFIP (Argentina's IRS) web services: electronic invoice, tax bonus, insurance, foreign trade, agriculture, customs, etc. (http://code.google.com/p/pyafipws/wiki/ProjectSummary)
 
 Now it has been extended to support other webservices like Currency Exchange Control and TrazaMed (National Traceability of Medical Drugs Program)
 
 Also, includes Server side support (a generic dispatcher, in order to be exposed from web2py service framework, adaptable to other webservers, including examples for standalone WSGI and django)
 
-Source Code originally available on [GoogleCode](https://code.google.com/p/py3simplesoap)
+Source Code originally available on [GoogleCode](https://code.google.com/p/pysimplesoap)
 
 
 Testing
 -------
 
-     python -m unittest discover -s tests -p "*_test.py"
+Using Python 2.7+:
+
+    python -m unittest discover
+
+Using older Python versions:
+
+    python -m unittest tests/suite.py
+
+Code coverage:
+
+    sudo pip install coverage
+    coverage run tests/suite.py
+    coverage report -m
+    coverage html
+
 
 Support
 -------
 
-For community support, please fell free to fill an [issue](https://github.com/py3simplesoap/py3simplesoap/issues/new) or send an email to [soap@python.org](https://mail.python.org/mailman/listinfo/soap).
+For community support, please fell free to fill an [issue](https://github.com/pysimplesoap/pysimplesoap/issues/new) or send an email to [soap@python.org](https://mail.python.org/mailman/listinfo/soap).
 Please do not add comment to wiki pages if you have technical questions.
 
-For priority commercial technical support, you can contact [Mariano Reingart](mailto:reingart@gmail.com) (project creator and main maintainer).
+For priority commercial technical support, you can contact [Mariano Reingart](mailto:reingart@gmail.com) (project creator and main maintainer, see [AUTHORS](AUTHORS.md) for more info).
```

### Comparing `py3simplesoap-0.10.18/py3simplesoap/client.py` & `py3simplesoap-0.2/py3simplesoap/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,25 +15,22 @@
 __author__ = "Mariano Reingart (reingart@gmail.com)"
 __copyright__ = "Copyright (C) 2008 Mariano Reingart"
 __license__ = "LGPL 3.0"
 __version__ = "1.08.14"
 
 TIMEOUT = 60
 
-import sys
-if sys.version > '3':
-    unicode = str
-
 import pickle as pickle
 import hashlib
 import logging
 import os
 import tempfile
 import urllib.request, urllib.error, urllib.parse
 import warnings
+import xml.dom.minidom as p_xml
 from urllib.parse import urlsplit
 from .simplexml import SimpleXMLElement, TYPE_MAP, REVERSE_TYPE_MAP, OrderedDict
 from .transport import get_http_wrapper, set_http_wrapper, get_Http
 
 log = logging.getLogger(__name__)
 logging.basicConfig(format='%(levelname)s:%(message)s', level=logging.WARNING)
 
@@ -46,24 +43,17 @@
 
     def __str__(self):
         return self.__unicode__().encode("ascii", "ignore")
 
     def __unicode__(self):
         return '%s: %s' % (self.faultcode, self.faultstring)
 
-    if sys.version > '3':
-        __str__ = __unicode__
-    else:
-        def __str__(self):
-            return self.__unicode__().encode('ascii', 'ignore')
-
     def __repr__(self):
-        return "SoapFault(faultcode = %s, faultstring %s, detail = %s)" % (repr(self.faultcode),
-                                                                           repr(self.faultstring),
-                                                                           repr(self.detail))
+        return "SoapFault(%s, %s)" % (repr(self.faultcode), 
+                                       repr(self.faultstring))
 
 
 # soap protocol specification & namespace
 soap_namespaces = dict(
     soap11="http://schemas.xmlsoap.org/soap/envelope/",
     soap="http://schemas.xmlsoap.org/soap/envelope/",
     soapenv="http://schemas.xmlsoap.org/soap/envelope/",
@@ -242,35 +232,51 @@
         location = self.location
                 
         if self.services:
             soap_action = self.action 
         else:
             soap_action = self.action + method
 
+        # prevent unicode encoding error (implicit conversions):
+        if not soap_action:
+            soap_action = str(soap_action)
+        elif not isinstance(soap_action, str):
+            soap_action = soap_action.decode("utf8")
+        if not isinstance(location, str):
+            location = location.decode("utf8")
+        if not isinstance(xml, str):
+            xml = xml.decode("utf8")
+        elif isinstance(xml, str):
+            xml = xml #.decode("latin1").encode("utf8")  # asume encoding ok
+
         headers={
             'Content-type': 'text/xml; charset="UTF-8"',
             'Content-length': str(len(xml)),
             "SOAPAction": "\"%s\"" % (soap_action)
         }
         headers.update(self.http_headers)
-        headers['User-Agent'] = 'Mozilla/5.0 (Windows NT 6.1; Win64; x64)'
         log.info("POST %s" % location)
         log.info("Headers: %s" % headers)
-        
         if self.trace:
             print("-"*80)
             print("POST %s" % location)
             print('\n'.join(["%s: %s" % (k,v) for k,v in list(headers.items())]))
             print("\n%s" % xml)
         
         response, content = self.http.request(
             location, "POST", body=xml, headers=headers)
         self.response = response
         self.content = content
-        
+
+        log.warn("###_XML REQUEST_### : " + str(xml))
+        #docu = p_xml.parseString(content.decode("utf-8"))
+        #pettrydocu = docu.toprettyxml(encoding='UTF-8')
+        log.warn("###_XML RESPONSE_### : " + p_xml.parseString(content.decode()).toprettyxml())
+
+
         if self.trace: 
             print() 
             print('\n'.join(["%s: %s" % (k,v) for k,v in list(response.items())]))
             print(content.decode("utf8", "ignore").encode("ascii", "replace"))
             print("="*80)
         return content
 
@@ -450,16 +456,15 @@
             else:
                 if url_scheme == 'file':
                     log.info("Fetching url %s using urllib2" % (url, ))
                     f = urllib.request.urlopen(url)
                     xml = f.read()
                 else:
                     log.info("GET %s using %s" % (url, self.http._wrapper_version))
-                    response, xml = self.http.request(url, "GET", None, {
-                        'User-Agent': 'Mozilla/5.0 (Windows NT 6.1; Win64; x64)'})
+                    response, xml = self.http.request(url, "GET", None, {})
                 if cache:
                     log.info("Writing file %s" % (filename, ))
                     try:
                         if not os.path.isdir(cache):
                             os.makedirs(cache)
                         f = open(filename, "wb")
                         f.write(xml)
```

### Comparing `py3simplesoap-0.10.18/py3simplesoap/server.py` & `py3simplesoap-0.2/py3simplesoap/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -480,19 +480,19 @@
         start_response('200 OK', [('Content-Type', 'text/xml'), ('Content-Length', str(len(response)))])
         return [response]
 
 if __name__=="__main__":
     import sys
 
     dispatcher = SoapDispatcher(
-        name = "py3simplesoapSample",
+        name = "PySimpleSoapSample",
         location = "http://localhost:8008/",
         action = 'http://localhost:8008/', # SOAPAction
-        namespace = "http://example.com/py3simplesoapsamle/", prefix="ns0",
-        documentation = 'Example soap service using py3simplesoap',
+        namespace = "http://example.com/pysimplesoapsamle/", prefix="ns0",
+        documentation = 'Example soap service using PySimpleSoap',
         trace = True,
         ns = True)
     
     def adder(p,c, dt=None):
         "Add several values"
         print(c[0]['d'],c[1]['d'], end=' ')
         import datetime
```

### Comparing `py3simplesoap-0.10.18/py3simplesoap/simplexml.py` & `py3simplesoap-0.2/py3simplesoap/simplexml.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,19 @@
 import logging
 import re
 import time
 import warnings
 import xml.dom.minidom
 from decimal import Decimal
 
+# Utility functions used for marshalling, moved aside for readability
+from .helpers import TYPE_MAP, TYPE_MARSHAL_FN, TYPE_UNMARSHAL_FN, \
+                     REVERSE_TYPE_MAP, Struct, Date, Decimal
+
+
 log = logging.getLogger(__name__)
 logging.basicConfig(format='%(levelname)s:%(message)s', level=logging.WARNING)
 
 DEBUG = False
 
 try:
     _strptime = datetime.datetime.strptime
@@ -82,53 +87,20 @@
 double = Alias(float,'double')
 integer = Alias(int,'integer')
 long = Alias(int,'long')
 DateTime = datetime.datetime
 Date = datetime.date
 Time = datetime.time
 
-# Define convertion function (python type): xml schema type
-TYPE_MAP = {
-    str:'string',
-    str:'string',
-    bool:'boolean', 
-    short:'short', 
-    byte:'byte',
-    int:'int', 
-    long:'long',
-    integer:'integer', 
-    float:'float', 
-    double:'double',
-    Decimal:'decimal',
-    datetime.datetime:'dateTime', 
-    datetime.date:'date',
-}
-TYPE_MARSHAL_FN = {
-    datetime.datetime:datetime_m, 
-    datetime.date:date_m,
-    bool:bool_m
-}
-TYPE_UNMARSHAL_FN = {
-    datetime.datetime:datetime_u, 
-    datetime.date:date_u,
-    bool:bool_u, 
-    str:str,
-}
-
-REVERSE_TYPE_MAP = dict([(v,k) for k,v in list(TYPE_MAP.items())])
-REVERSE_TYPE_MAP.update({
-    'base64Binary': base64.b64decode,
-})
 
 
 from collections import OrderedDict as ordered_dict
 class OrderedDict(ordered_dict):
     "Minimal ordered dictionary for xsd:sequences"
     def __init__(self):
-        super(OrderedDict, self).__init__()
         self.__keys = []
         self.array = False
     def __setitem__(self, key, value):
         if key not in self.__keys:
             self.__keys.append(key)
         ordered_dict.__setitem__(self, key, value)
     def insert(self, key, value, index=0):
@@ -240,17 +212,17 @@
         "Add an xml comment to this child"
         comment = self.__document.createComment(data)
         self._element.appendChild(comment)
 
     def as_xml(self, filename=None, pretty=False):
         "Return the XML representation of the document"
         if not pretty:
-            return self.__document.toxml('UTF-8').decode('UTF-8')
+            return self.__document.toxml('UTF-8')
         else:
-            return self.__document.toprettyxml(encoding='UTF-8').decode('UTF-8')
+            return self.__document.toprettyxml(encoding='UTF-8')
 
     def __repr__(self):
         "Return the XML representation of this tag"
         return self._element.toxml('UTF-8')
 
     def get_name(self):
         "Return the tag name of this node"
@@ -595,17 +567,17 @@
             # process inner tags (values):
             for i, item in enumerate(value):
                 subtypes = types[0] if isinstance(types, list) else None
                 child.marshall(name, item, False, add_comments=add_comments, ns=ns, types=subtypes)
                 # "jetty" arrays: add new base node (if not last) -see abobe-
                 # TODO: this could be an issue for some arrays of single values
                 if isinstance(item, dict):
-                    if (len(item) > 1 or subtypes and len(subtypes) > 1 or
-                            (isinstance(subtypes, dict) and
-                             not isinstance(list(subtypes.values())[0], dict))):
+                    if (len(item) > 1 or len(subtypes)>1 or 
+                        (isinstance(subtypes, dict) and 
+                         not isinstance(list(subtypes.values())[0], dict))): 
                         if i < len(value) - 1:
                             # new parent tag for next item:
                             child = self.add_child(name, ns=ns)
         elif isinstance(value, str): # do not convert strings or unicodes
             self.add_child(name, value,ns=ns)
         elif value is None: # sent a empty tag?
             self.add_child(name, ns=ns)
```

### Comparing `py3simplesoap-0.10.18/py3simplesoap/transport.py` & `py3simplesoap-0.2/py3simplesoap/transport.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 import urllib.request, urllib.error, urllib.parse
 from urllib.parse import urlparse
 import tempfile
 from .simplexml import SimpleXMLElement, TYPE_MAP, OrderedDict
 import logging
 import warnings
 import time
-from distutils.version import LooseVersion
 
 # Required in Python2.6+ to force SSLv3:
 try:
     import ssl
 except:
     ssl = None
 
@@ -68,17 +67,17 @@
             kwargs = {}
             if proxy:
                 import socks
                 kwargs['proxy_info'] = httplib2.ProxyInfo(proxy_type=socks.PROXY_TYPE_HTTP, **proxy)
                 print("using proxy", proxy)
 
             # set optional parameters according supported httplib2 version
-            if LooseVersion(httplib2.__version__) >= LooseVersion('0.3.0'):
+            if httplib2.__version__ >= '0.3.0':
                 kwargs['timeout'] = timeout
-            if LooseVersion(httplib2.__version__) >= LooseVersion('0.7.0'):
+            if httplib2.__version__ >= '0.7.0':
                 kwargs['disable_ssl_certificate_validation'] = cacert is None
                 kwargs['ca_certs'] = cacert
             # downgrade to highest compatible protocol version available:
             if ssl:
                 # SSLv3 is obsolete, use only if requested
                 if USE_SSLv3:
                     self.ssl_version = ssl.PROTOCOL_SSLv3
@@ -112,27 +111,27 @@
             try:
                 if DEBUG:
                     print("Connecting to https://%s:%s%s using protocol %s" % (
                         conn.host, conn.port, request_uri, ssl.get_protocol_name(self.ssl_version)))
                 ##if False and DEBUG and self.ssl_version != ssl.PROTOCOL_TLSv1:
                 ##    raise ssl.SSLError
                 return httplib2.Http._conn_request(self, conn, request_uri, method, body, headers)
-            except (ssl.SSLError, IOError) as e:
+            except (ssl.SSLError, httplib2.SSLHandshakeError) as e:
                 # fallback to previous protocols
                 if hasattr(ssl, "PROTOCOL_TLSv1_2") and self.ssl_version == ssl.PROTOCOL_TLSv1_2:
                     new_ssl_version = ssl.PROTOCOL_TLSv1
                 ##elif self.ssl_version == ssl.PROTOCOL_TLSv1:
                 ##    new_ssl_version = ssl.PROTOCOL_SSLv3
                 ##elif self.ssl_version == ssl.PROTOCOL_SSLv3:
                 ##    new_ssl_version = ssl.PROTOCOL_SSLv23
                 else:
                     raise
                 if DEBUG:
-                    warnings.warn("Protocol %s failed: %s; downgrading to %s" %
-                                (ssl.get_protocol_name(self.ssl_version), e,
+                    warnings.warn("Protocol %s failed: %s; downgrading to %s" % 
+                                (ssl.get_protocol_name(self.ssl_version), e, 
                                  ssl.get_protocol_name(new_ssl_version)))
                 self.ssl_version = new_ssl_version
                 return Httplib2Transport._conn_request(self, conn, request_uri, method, body, headers)
 
     _http_connectors['httplib2'] = Httplib2Transport
     _http_facilities.setdefault('proxy', []).append('httplib2')
     _http_facilities.setdefault('cacert', []).append('httplib2')
@@ -143,41 +142,40 @@
 
 #
 # urllib2 support.
 #
 import urllib.request, urllib.error, urllib.parse
 class urllib2Transport(TransportBase):
     _wrapper_version = "urllib2"
-    _wrapper_name = 'urllib2'
+    _wrapper_name = 'urllib2' 
     def __init__(self, timeout=None, proxy=None, cacert=None, sessions=False):
         import sys
         if (timeout is not None) and not self.supports_feature('timeout'):
             raise RuntimeError('timeout is not supported with urllib2 transport')
         if proxy:
             raise RuntimeError('proxy is not supported with urllib2 transport')
         if cacert:
             raise RuntimeError('cacert is not support with urllib2 transport')
 
         self.request_opener = urllib.request.urlopen
         if sessions:
             from http.cookiejar import CookieJar
             opener = urllib.request.build_opener(urllib.request.HTTPCookieProcessor(CookieJar()))
             self.request_opener = opener.open
-
+            
         self._timeout = timeout
 
     def request(self, url, method="GET", body=None, headers={}):
         req = urllib.request.Request(url, body, headers)
         try:
             f = self.request_opener(req, timeout=self._timeout)
-            return f.info(), f.read()
         except urllib.error.HTTPError as f:
             if f.code != 500:
                 raise
-            return f.info(), f.read()
+        return f.info(), f.read()
 
 _http_connectors['urllib2'] = urllib2Transport
 _http_facilities.setdefault('sessions', []).append('urllib2')
 
 import sys
 if sys.version_info >= (2,6):
     _http_facilities.setdefault('timeout', []).append('urllib2')
@@ -197,18 +195,18 @@
     except ImportError:
         from io import StringIO
 
     class pycurlTransport(TransportBase):
         _wrapper_version = pycurl.version
         _wrapper_name = 'pycurl'
         def __init__(self, timeout, proxy=None, cacert=None, sessions=False):
-            self.timeout = timeout
+            self.timeout = timeout 
             self.proxy = proxy or {}
             self.cacert = cacert
-
+               
         def request(self, url, method, body, headers):
             c = pycurl.Curl()
             c.setopt(pycurl.URL, str(url))
             if 'proxy_host' in self.proxy:
                 c.setopt(pycurl.PROXY, self.proxy['proxy_host'])
             if 'proxy_port' in self.proxy:
                 c.setopt(pycurl.PROXYPORT, self.proxy['proxy_port'])
@@ -216,26 +214,26 @@
                 c.setopt(pycurl.PROXYUSERPWD, "%(proxy_user)s:%(proxy_pass)s" % self.proxy)
             self.buf = StringIO()
             c.setopt(pycurl.WRITEFUNCTION, self.buf.write)
             #c.setopt(pycurl.READFUNCTION, self.read)
             #self.body = StringIO(body)
             #c.setopt(pycurl.HEADERFUNCTION, self.header)
             if self.cacert:
-                c.setopt(c.CAINFO, str(self.cacert))
+                c.setopt(c.CAINFO, str(self.cacert)) 
             if USE_SSLv3:
                 c.setopt(pycurl.SSLVERSION, pycurl.SSLVERSION_SSLv3)
             elif USE_SSLv3 is not None:
                 c.setopt(pycurl.SSLVERSION, pycurl.SSLVERSION_TLSv1)
             c.setopt(pycurl.SSL_VERIFYPEER, self.cacert and 1 or 0)
             c.setopt(pycurl.SSL_VERIFYHOST, self.cacert and 2 or 0)
-            c.setopt(pycurl.CONNECTTIMEOUT, self.timeout/6)
+            c.setopt(pycurl.CONNECTTIMEOUT, self.timeout/6) 
             c.setopt(pycurl.TIMEOUT, self.timeout)
             if method=='POST':
                 c.setopt(pycurl.POST, 1)
-                c.setopt(pycurl.POSTFIELDS, body)
+                c.setopt(pycurl.POSTFIELDS, body)            
             if headers:
                 hdrs = ['%s: %s' % (str(k), str(v)) for k, v in list(headers.items())]
                 ##print hdrs
                 c.setopt(pycurl.HTTPHEADER, hdrs)
             c.perform()
             ##print "pycurl perform..."
             c.close()
@@ -245,18 +243,18 @@
     _http_facilities.setdefault('proxy', []).append('pycurl')
     _http_facilities.setdefault('cacert', []).append('pycurl')
     _http_facilities.setdefault('timeout', []).append('pycurl')
 
 
 class DummyTransport:
     "Testing class to load a xml response"
-
+    
     def __init__(self, xml_response):
         self.xml_response = xml_response
-
+        
     def request(self, location, method, body, headers):
         if False:
             print(method, location)
             print(headers)
             print(body)
         return {}, self.xml_response
 
@@ -301,13 +299,13 @@
 
 
 def get_Http():
     "Return current transport class"
     global Http
     return Http
 
-
+    
 # define the default HTTP connection class (it can be changed at runtime!):
 set_http_wrapper()
```

