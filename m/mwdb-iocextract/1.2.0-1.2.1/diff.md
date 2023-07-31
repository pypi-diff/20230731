# Comparing `tmp/mwdb-iocextract-1.2.0.tar.gz` & `tmp/mwdb-iocextract-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwdb-iocextract-1.2.0.tar", last modified: Mon Jul 17 13:01:33 2023, max compression
+gzip compressed data, was "mwdb-iocextract-1.2.1.tar", last modified: Mon Jul 31 10:42:20 2023, max compression
```

## Comparing `mwdb-iocextract-1.2.0.tar` & `mwdb-iocextract-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:01:33.893171 mwdb-iocextract-1.2.0/
--rw-r--r--   0 root         (0) root         (0)     7109 2023-07-17 13:01:33.893171 mwdb-iocextract-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6737 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:01:33.892171 mwdb-iocextract-1.2.0/mwdb_iocextract.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7109 2023-07-17 13:01:33.000000 mwdb-iocextract-1.2.0/mwdb_iocextract.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      351 2023-07-17 13:01:33.000000 mwdb-iocextract-1.2.0/mwdb_iocextract.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 13:01:33.000000 mwdb-iocextract-1.2.0/mwdb_iocextract.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-17 13:01:33.000000 mwdb-iocextract-1.2.0/mwdb_iocextract.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-17 13:01:33.000000 mwdb-iocextract-1.2.0/mwdb_iocextract.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       74 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       43 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-17 13:01:33.893171 mwdb-iocextract-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      765 2023-07-17 12:43:41.000000 mwdb-iocextract-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 13:01:33.893171 mwdb-iocextract-1.2.0/src/
--rw-r--r--   0 root         (0) root         (0)      364 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.0/src/__init__.py
--rw-r--r--   0 root         (0) root         (0)      310 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.0/src/api.py
--rw-r--r--   0 root         (0) root         (0)      342 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.0/src/errors.py
--rw-r--r--   0 root         (0) root         (0)    12444 2023-07-17 12:02:11.000000 mwdb-iocextract-1.2.0/src/model.py
--rw-r--r--   0 root         (0) root         (0)    12160 2023-07-17 12:02:11.000000 mwdb-iocextract-1.2.0/src/modules.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.0/src/run.py
--rw-r--r--   0 root         (0) root         (0)     1145 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.0/src/test_misp.py
+drwxr-xr-x   0 msm       (1000) users      (100)        0 2023-07-31 10:42:20.853353 mwdb-iocextract-1.2.1/
+-rw-r--r--   0 msm       (1000) users      (100)     7053 2023-07-31 10:42:20.853353 mwdb-iocextract-1.2.1/PKG-INFO
+-rw-r--r--   0 msm       (1000) users      (100)     6737 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.1/README.md
+drwxr-xr-x   0 msm       (1000) users      (100)        0 2023-07-31 10:42:20.852353 mwdb-iocextract-1.2.1/mwdb_iocextract.egg-info/
+-rw-r--r--   0 msm       (1000) users      (100)     7053 2023-07-31 10:42:20.000000 mwdb-iocextract-1.2.1/mwdb_iocextract.egg-info/PKG-INFO
+-rw-r--r--   0 msm       (1000) users      (100)      351 2023-07-31 10:42:20.000000 mwdb-iocextract-1.2.1/mwdb_iocextract.egg-info/SOURCES.txt
+-rw-r--r--   0 msm       (1000) users      (100)        1 2023-07-31 10:42:20.000000 mwdb-iocextract-1.2.1/mwdb_iocextract.egg-info/dependency_links.txt
+-rw-r--r--   0 msm       (1000) users      (100)       44 2023-07-31 10:42:20.000000 mwdb-iocextract-1.2.1/mwdb_iocextract.egg-info/requires.txt
+-rw-r--r--   0 msm       (1000) users      (100)       16 2023-07-31 10:42:20.000000 mwdb-iocextract-1.2.1/mwdb_iocextract.egg-info/top_level.txt
+-rw-r--r--   0 msm       (1000) users      (100)       74 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.1/pyproject.toml
+-rw-r--r--   0 msm       (1000) users      (100)       43 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.1/requirements.txt
+-rw-r--r--   0 msm       (1000) users      (100)      101 2023-07-31 10:42:20.853353 mwdb-iocextract-1.2.1/setup.cfg
+-rw-r--r--   0 msm       (1000) users      (100)      765 2023-07-31 10:41:29.000000 mwdb-iocextract-1.2.1/setup.py
+drwxr-xr-x   0 msm       (1000) users      (100)        0 2023-07-31 10:42:20.853353 mwdb-iocextract-1.2.1/src/
+-rw-r--r--   0 msm       (1000) users      (100)      364 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.1/src/__init__.py
+-rw-r--r--   0 msm       (1000) users      (100)      310 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.1/src/api.py
+-rw-r--r--   0 msm       (1000) users      (100)      342 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.1/src/errors.py
+-rw-r--r--   0 msm       (1000) users      (100)    12624 2023-07-31 10:41:18.000000 mwdb-iocextract-1.2.1/src/model.py
+-rw-r--r--   0 msm       (1000) users      (100)    12160 2023-07-17 12:02:11.000000 mwdb-iocextract-1.2.1/src/modules.py
+-rw-r--r--   0 msm       (1000) users      (100)      936 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.1/src/run.py
+-rw-r--r--   0 msm       (1000) users      (100)     1145 2023-07-13 12:15:28.000000 mwdb-iocextract-1.2.1/src/test_misp.py
```

### Comparing `mwdb-iocextract-1.2.0/PKG-INFO` & `mwdb-iocextract-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: mwdb-iocextract
-Version: 1.2.0
+Version: 1.2.1
 Summary: Mwdb config parser
-Home-page: UNKNOWN
 Author: CERT Polska
 Author-email: info@cert.pl
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # mwdb-iocextract
 
@@ -298,9 +295,7 @@
 
     for o in iocs.to_misp():
         event.add_object(o)
 
     misp = ExpandedPyMISP(MISP_URL, MISP_KEY, MISP_VERIFYCERT)
     misp.add_event(event)
 ```
-
-
```

### Comparing `mwdb-iocextract-1.2.0/README.md` & `mwdb-iocextract-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mwdb-iocextract-1.2.0/mwdb_iocextract.egg-info/PKG-INFO` & `mwdb-iocextract-1.2.1/mwdb_iocextract.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: mwdb-iocextract
-Version: 1.2.0
+Version: 1.2.1
 Summary: Mwdb config parser
-Home-page: UNKNOWN
 Author: CERT Polska
 Author-email: info@cert.pl
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # mwdb-iocextract
 
@@ -298,9 +295,7 @@
 
     for o in iocs.to_misp():
         event.add_object(o)
 
     misp = ExpandedPyMISP(MISP_URL, MISP_KEY, MISP_VERIFYCERT)
     misp.add_event(event)
 ```
-
-
```

### Comparing `mwdb-iocextract-1.2.0/setup.py` & `mwdb-iocextract-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fh:
     requirements = fh.read().split('\n')
 
 setuptools.setup(
     name="mwdb-iocextract",
-    version="1.2.0",
+    version="1.2.1",
     data_files=[('requirements.txt', ['requirements.txt'])],
     author="CERT Polska",
     author_email="info@cert.pl",
     package_dir={"mwdb_iocextract": "src"},
     packages=["mwdb_iocextract"],
     description="Mwdb config parser",
     long_description=long_description,
```

### Comparing `mwdb-iocextract-1.2.0/src/model.py` & `mwdb-iocextract-1.2.1/src/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import re
 from base64 import b64encode
 from enum import Enum
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Tuple, Union, cast
 from urllib.parse import urlparse
 
 from Cryptodome.PublicKey import RSA  # type: ignore
 from malduck import base64, rsa  # type: ignore
-from pymisp import MISPObject  # type: ignore
+from pymisp import MISPAttribute, MISPObject  # type: ignore
 
 from .errors import IocExtractError
 
 PUBKEY_PEM_TEMPLATE = (
     "-----BEGIN PUBLIC KEY-----\n{}\n-----END PUBLIC KEY-----"
 )
 
@@ -159,31 +159,34 @@
         else:
             misp_object_type = "domain-ip"
 
         obj = MISPObject(misp_object_type, standalone=False)
 
         # url-specific attributes
         if self.scheme:
-            obj.add_attribute("url", self.pretty_url)
+            url = cast(
+                MISPAttribute, obj.add_attribute("url", self.pretty_url)
+            )
+            url.add_tag(f"mwdb:location_type:{self.location_type.value}")
         if self.path:
             obj.add_attribute("resource_path", self.path)
         if self.url.fragment:
             obj.add_attribute("fragment", self.url.fragment)
         if self.query:
             obj.add_attribute("query_string", self.query)
 
         # generic attributes that apply to both url and domain-ip
         if self.ip:
-            a = obj.add_attribute("ip", self.ip)
-            if a is not None:
-                a.add_tag(f"mwdb:location_type:{self.location_type.value}")
+            ip = cast(MISPAttribute, obj.add_attribute("ip", self.ip))
+            ip.add_tag(f"mwdb:location_type:{self.location_type.value}")
         if self.domain:
-            a = obj.add_attribute("domain", self.domain)
-            if a is not None:
-                a.add_tag(f"mwdb:location_type:{self.location_type.value}")
+            domain = cast(
+                MISPAttribute, obj.add_attribute("domain", self.domain)
+            )
+            domain.add_tag(f"mwdb:location_type:{self.location_type.value}")
         if self.port:
             obj.add_attribute("port", self.port)
 
         return obj
 
     def prettyprint(self) -> str:
         """Pretty print for debugging"""
@@ -290,27 +293,27 @@
         """MISP JSON output"""
         to_return = []
         for rsa_key in self.rsa_keys:
             to_return.append(rsa_key.to_misp())
         for ecdsa_curve in self.ecdsa_curves:
             to_return.append(ecdsa_curve.to_misp())
         if self.keys:
-            crypto_obj = MISPObject("crypto-material", standalone=False)
             for k in self.keys:
+                crypto_obj = MISPObject("crypto-material", standalone=False)
                 crypto_obj.add_attribute("type", k[0])
                 crypto_obj.add_attribute("generic-symmetric-key", k[1])
                 to_return.append(crypto_obj)
         if self.passwords:
-            credential_obj = MISPObject("credential", standalone=False)
             for password in self.passwords:
+                credential_obj = MISPObject("credential", standalone=False)
                 credential_obj.add_attribute("password", password)
                 to_return.append(credential_obj)
         if self.mutexes:
-            mutex_obj = MISPObject("mutex", standalone=False)
             for mutex in self.mutexes:
+                mutex_obj = MISPObject("mutex", standalone=False)
                 mutex_obj.add_attribute("name", mutex)
                 to_return.append(mutex_obj)
         for netloc in self.network_locations:
             to_return.append(netloc.to_misp())
         # TODO self.dropped_filenames
         for email in self.emails_to:
             obj = MISPObject("email", standalone=False)
```

### Comparing `mwdb-iocextract-1.2.0/src/modules.py` & `mwdb-iocextract-1.2.1/src/modules.py`

 * *Files identical despite different names*

### Comparing `mwdb-iocextract-1.2.0/src/run.py` & `mwdb-iocextract-1.2.1/src/run.py`

 * *Files identical despite different names*

### Comparing `mwdb-iocextract-1.2.0/src/test_misp.py` & `mwdb-iocextract-1.2.1/src/test_misp.py`

 * *Files identical despite different names*

