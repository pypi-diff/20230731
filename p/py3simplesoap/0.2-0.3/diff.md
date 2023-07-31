# Comparing `tmp/py3simplesoap-0.2.tar.gz` & `tmp/py3simplesoap-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3simplesoap-0.2.tar", last modified: Mon Jul 31 03:35:00 2023, max compression
+gzip compressed data, was "py3simplesoap-0.3.tar", last modified: Mon Jul 31 03:59:49 2023, max compression
```

## Comparing `py3simplesoap-0.2.tar` & `py3simplesoap-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 far        (501) staff       (20)        0 2023-07-31 03:35:00.212236 py3simplesoap-0.2/
--rw-r--r--   0 far        (501) staff       (20)      670 2023-07-31 03:35:00.212312 py3simplesoap-0.2/PKG-INFO
--rw-r--r--   0 far        (501) staff       (20)     4074 2023-07-31 03:30:58.000000 py3simplesoap-0.2/README.md
-drwxr-xr-x   0 far        (501) staff       (20)        0 2023-07-31 03:35:00.210804 py3simplesoap-0.2/py3simplesoap/
--rw-r--r--   0 far        (501) staff       (20)      150 2023-07-31 03:30:58.000000 py3simplesoap-0.2/py3simplesoap/__init__.py
--rw-r--r--   0 far        (501) staff       (20)    38671 2023-07-31 03:30:58.000000 py3simplesoap-0.2/py3simplesoap/client.py
--rw-r--r--   0 far        (501) staff       (20)    28906 2023-07-31 03:30:58.000000 py3simplesoap-0.2/py3simplesoap/helpers.py
--rw-r--r--   0 far        (501) staff       (20)    22991 2023-07-31 03:30:58.000000 py3simplesoap-0.2/py3simplesoap/server.py
--rw-r--r--   0 far        (501) staff       (20)    24162 2023-07-31 03:30:58.000000 py3simplesoap-0.2/py3simplesoap/simplexml.py
--rw-r--r--   0 far        (501) staff       (20)    12080 2023-07-31 03:30:58.000000 py3simplesoap-0.2/py3simplesoap/transport.py
-drwxr-xr-x   0 far        (501) staff       (20)        0 2023-07-31 03:35:00.212045 py3simplesoap-0.2/py3simplesoap.egg-info/
--rw-r--r--   0 far        (501) staff       (20)      670 2023-07-31 03:35:00.000000 py3simplesoap-0.2/py3simplesoap.egg-info/PKG-INFO
--rw-r--r--   0 far        (501) staff       (20)      329 2023-07-31 03:35:00.000000 py3simplesoap-0.2/py3simplesoap.egg-info/SOURCES.txt
--rw-r--r--   0 far        (501) staff       (20)        1 2023-07-31 03:35:00.000000 py3simplesoap-0.2/py3simplesoap.egg-info/dependency_links.txt
--rw-r--r--   0 far        (501) staff       (20)       14 2023-07-31 03:35:00.000000 py3simplesoap-0.2/py3simplesoap.egg-info/top_level.txt
--rw-r--r--   0 far        (501) staff       (20)      108 2023-07-31 03:35:00.212600 py3simplesoap-0.2/setup.cfg
--rw-r--r--   0 far        (501) staff       (20)      876 2023-07-31 03:34:48.000000 py3simplesoap-0.2/setup.py
+drwxr-xr-x   0 far        (501) staff       (20)        0 2023-07-31 03:59:49.960391 py3simplesoap-0.3/
+-rw-r--r--   0 far        (501) staff       (20)      670 2023-07-31 03:59:49.960513 py3simplesoap-0.3/PKG-INFO
+-rw-r--r--   0 far        (501) staff       (20)     4074 2023-07-31 03:30:58.000000 py3simplesoap-0.3/README.md
+drwxr-xr-x   0 far        (501) staff       (20)        0 2023-07-31 03:59:49.959559 py3simplesoap-0.3/py3simplesoap/
+-rw-r--r--   0 far        (501) staff       (20)      150 2023-07-31 03:30:58.000000 py3simplesoap-0.3/py3simplesoap/__init__.py
+-rw-r--r--   0 far        (501) staff       (20)    38671 2023-07-31 03:30:58.000000 py3simplesoap-0.3/py3simplesoap/client.py
+-rw-r--r--   0 far        (501) staff       (20)    28906 2023-07-31 03:30:58.000000 py3simplesoap-0.3/py3simplesoap/helpers.py
+-rw-r--r--   0 far        (501) staff       (20)    22991 2023-07-31 03:30:58.000000 py3simplesoap-0.3/py3simplesoap/server.py
+-rw-r--r--   0 far        (501) staff       (20)    24288 2023-07-31 03:58:38.000000 py3simplesoap-0.3/py3simplesoap/simplexml.py
+-rw-r--r--   0 far        (501) staff       (20)    12080 2023-07-31 03:30:58.000000 py3simplesoap-0.3/py3simplesoap/transport.py
+drwxr-xr-x   0 far        (501) staff       (20)        0 2023-07-31 03:59:49.960237 py3simplesoap-0.3/py3simplesoap.egg-info/
+-rw-r--r--   0 far        (501) staff       (20)      670 2023-07-31 03:59:49.000000 py3simplesoap-0.3/py3simplesoap.egg-info/PKG-INFO
+-rw-r--r--   0 far        (501) staff       (20)      329 2023-07-31 03:59:49.000000 py3simplesoap-0.3/py3simplesoap.egg-info/SOURCES.txt
+-rw-r--r--   0 far        (501) staff       (20)        1 2023-07-31 03:59:49.000000 py3simplesoap-0.3/py3simplesoap.egg-info/dependency_links.txt
+-rw-r--r--   0 far        (501) staff       (20)       14 2023-07-31 03:59:49.000000 py3simplesoap-0.3/py3simplesoap.egg-info/top_level.txt
+-rw-r--r--   0 far        (501) staff       (20)      108 2023-07-31 03:59:49.960815 py3simplesoap-0.3/setup.cfg
+-rw-r--r--   0 far        (501) staff       (20)      876 2023-07-31 03:59:38.000000 py3simplesoap-0.3/setup.py
```

### Comparing `py3simplesoap-0.2/PKG-INFO` & `py3simplesoap-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3simplesoap
-Version: 0.2
+Version: 0.3
 Summary: pysimplesoap for python3
 Home-page: https://github.com/odoo-mastercore/pysimplesoap
 Download-URL: https://github.com/odoo-mastercore/pysimplesoap/tarball/0.1
 Author: Mastercore
 Author-email: far@mastercore.net
 Keywords: py3simplesoap,py3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `py3simplesoap-0.2/README.md` & `py3simplesoap-0.3/README.md`

 * *Files identical despite different names*

### Comparing `py3simplesoap-0.2/py3simplesoap/client.py` & `py3simplesoap-0.3/py3simplesoap/client.py`

 * *Files identical despite different names*

### Comparing `py3simplesoap-0.2/py3simplesoap/helpers.py` & `py3simplesoap-0.3/py3simplesoap/helpers.py`

 * *Files identical despite different names*

### Comparing `py3simplesoap-0.2/py3simplesoap/server.py` & `py3simplesoap-0.3/py3simplesoap/server.py`

 * *Files identical despite different names*

### Comparing `py3simplesoap-0.2/py3simplesoap/simplexml.py` & `py3simplesoap-0.3/py3simplesoap/simplexml.py`

 * *Files 2% similar despite different names*

```diff
@@ -434,14 +434,16 @@
             except (KeyError, ) as e:
                 if node.get_namespace_uri("soapenc"):
                     fn = None # ignore multirefs!
                 elif 'xsi:type' in list(node.attributes().keys()):
                     xsd_type = node['xsi:type'].split(":")[1]
                     fn = REVERSE_TYPE_MAP[xsd_type]
                 elif strict:
+                    log.debug('ESTO ES EL FALLO %s', str(fn))
+                    log.debug('ESTO ES EL FALLO %s', str(node))
                     raise TypeError("Tag: %s invalid (type not found)" % (name,))
                 else:
                     # if not strict, use default type conversion
                     fn = str
             
             if isinstance(fn, list):
                 # append to existing list (if any) - unnested dict arrays -
```

### Comparing `py3simplesoap-0.2/py3simplesoap/transport.py` & `py3simplesoap-0.3/py3simplesoap/transport.py`

 * *Files identical despite different names*

### Comparing `py3simplesoap-0.2/py3simplesoap.egg-info/PKG-INFO` & `py3simplesoap-0.3/py3simplesoap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3simplesoap
-Version: 0.2
+Version: 0.3
 Summary: pysimplesoap for python3
 Home-page: https://github.com/odoo-mastercore/pysimplesoap
 Download-URL: https://github.com/odoo-mastercore/pysimplesoap/tarball/0.1
 Author: Mastercore
 Author-email: far@mastercore.net
 Keywords: py3simplesoap,py3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `py3simplesoap-0.2/setup.py` & `py3simplesoap-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
   name = 'py3simplesoap',
   packages = ['py3simplesoap'], # this must be the same as the name above
-  version = '0.2',
+  version = '0.3',
   description = 'pysimplesoap for python3',
   long_description = 'pysimplesoap for python3',
   author = 'Mastercore',
   author_email = 'far@mastercore.net',
   # use the URL to the github repo
   url = 'https://github.com/odoo-mastercore/pysimplesoap',
   download_url = 'https://github.com/odoo-mastercore/pysimplesoap/tarball/0.1',
```

