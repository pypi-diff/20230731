# Comparing `tmp/madrigalWeb-3.2.3.tar.gz` & `tmp/madrigalWeb-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/madrigalWeb-3.2.3.tar", last modified: Tue Nov  8 21:26:38 2022, max compression
+gzip compressed data, was "dist/madrigalWeb-3.2.4.tar", last modified: Mon Jul 31 20:04:21 2023, max compression
```

## Comparing `madrigalWeb-3.2.3.tar` & `madrigalWeb-3.2.4.tar`

### file list

```diff
@@ -1,16 +1,23 @@
-drwxr-xr-x   0 brideout   (501) staff       (20)        0 2022-11-08 21:26:38.000000 madrigalWeb-3.2.3/
--rw-r--r--   0 brideout   (501) staff       (20)      268 2022-11-08 21:26:38.000000 madrigalWeb-3.2.3/PKG-INFO
--rw-r--r--   0 brideout   (501) staff       (20)      345 2020-01-21 16:31:52.000000 madrigalWeb-3.2.3/README
-drwxr-xr-x   0 brideout   (501) staff       (20)        0 2022-11-08 21:26:38.000000 madrigalWeb-3.2.3/documentation/
--rw-r--r--   0 brideout   (501) staff       (20)     1944 2020-01-21 16:31:52.000000 madrigalWeb-3.2.3/documentation/madrigal.css
--rw-r--r--   0 brideout   (501) staff       (20)   343759 2022-05-25 14:52:46.000000 madrigalWeb-3.2.3/documentation/madrigalWeb.html
--rw-r--r--   0 brideout   (501) staff       (20)    40400 2021-04-22 17:40:23.000000 madrigalWeb-3.2.3/documentation/python_scripts.html
-drwxr-xr-x   0 brideout   (501) staff       (20)        0 2022-11-08 21:26:38.000000 madrigalWeb-3.2.3/madrigalWeb/
--rw-r--r--   0 brideout   (501) staff       (20)      312 2020-01-21 16:31:52.000000 madrigalWeb-3.2.3/madrigalWeb/__init__.py
-drwxr-xr-x   0 brideout   (501) staff       (20)        0 2022-11-08 21:26:38.000000 madrigalWeb-3.2.3/madrigalWeb/examples/
--rw-r--r--   0 brideout   (501) staff       (20)     4165 2021-12-17 15:52:40.000000 madrigalWeb-3.2.3/madrigalWeb/examples/exampleMadrigalWebServices.py
--rw-r--r--   0 brideout   (501) staff       (20)     8399 2020-10-02 20:05:22.000000 madrigalWeb-3.2.3/madrigalWeb/globalCitation.py
--rw-r--r--   0 brideout   (501) staff       (20)    25858 2022-09-19 18:31:01.000000 madrigalWeb-3.2.3/madrigalWeb/globalDownload.py
--rw-r--r--   0 brideout   (501) staff       (20)    35394 2021-04-22 17:55:08.000000 madrigalWeb-3.2.3/madrigalWeb/globalIsprint.py
--rw-r--r--   0 brideout   (501) staff       (20)   104939 2022-11-08 21:25:02.000000 madrigalWeb-3.2.3/madrigalWeb/madrigalWeb.py
--rw-r--r--   0 brideout   (501) staff       (20)      659 2022-11-08 21:23:40.000000 madrigalWeb-3.2.3/setup.py
+drwxr-xr-x   0 brideout   (501) staff       (20)        0 2023-07-31 20:04:21.000000 madrigalWeb-3.2.4/
+-rw-r--r--   0 brideout   (501) staff       (20)       56 2020-01-21 16:31:52.000000 madrigalWeb-3.2.4/MANIFEST.in
+-rw-r--r--   0 brideout   (501) staff       (20)      257 2023-07-31 20:04:21.000000 madrigalWeb-3.2.4/PKG-INFO
+-rw-r--r--   0 brideout   (501) staff       (20)      345 2020-01-21 16:31:52.000000 madrigalWeb-3.2.4/README
+drwxr-xr-x   0 brideout   (501) staff       (20)        0 2023-07-31 20:04:21.000000 madrigalWeb-3.2.4/documentation/
+-rw-r--r--   0 brideout   (501) staff       (20)     1944 2020-01-21 16:31:52.000000 madrigalWeb-3.2.4/documentation/madrigal.css
+-rw-r--r--   0 brideout   (501) staff       (20)   343759 2022-05-25 14:52:46.000000 madrigalWeb-3.2.4/documentation/madrigalWeb.html
+-rw-r--r--   0 brideout   (501) staff       (20)    40400 2021-04-22 17:40:23.000000 madrigalWeb-3.2.4/documentation/python_scripts.html
+drwxr-xr-x   0 brideout   (501) staff       (20)        0 2023-07-31 20:04:21.000000 madrigalWeb-3.2.4/madrigalWeb/
+-rw-r--r--   0 brideout   (501) staff       (20)      312 2020-01-21 16:31:52.000000 madrigalWeb-3.2.4/madrigalWeb/__init__.py
+drwxr-xr-x   0 brideout   (501) staff       (20)        0 2023-07-31 20:04:21.000000 madrigalWeb-3.2.4/madrigalWeb/examples/
+-rw-r--r--   0 brideout   (501) staff       (20)     4165 2021-12-17 15:52:40.000000 madrigalWeb-3.2.4/madrigalWeb/examples/exampleMadrigalWebServices.py
+-rw-r--r--   0 brideout   (501) staff       (20)     8399 2020-10-02 20:05:22.000000 madrigalWeb-3.2.4/madrigalWeb/globalCitation.py
+-rw-r--r--   0 brideout   (501) staff       (20)    25858 2023-07-31 18:20:42.000000 madrigalWeb-3.2.4/madrigalWeb/globalDownload.py
+-rw-r--r--   0 brideout   (501) staff       (20)    35394 2021-04-22 17:55:08.000000 madrigalWeb-3.2.4/madrigalWeb/globalIsprint.py
+-rw-r--r--   0 brideout   (501) staff       (20)   104922 2023-07-31 20:03:10.000000 madrigalWeb-3.2.4/madrigalWeb/madrigalWeb.py
+drwxr-xr-x   0 brideout   (501) staff       (20)        0 2023-07-31 20:04:21.000000 madrigalWeb-3.2.4/madrigalWeb.egg-info/
+-rw-r--r--   0 brideout   (501) staff       (20)      257 2023-07-31 20:04:20.000000 madrigalWeb-3.2.4/madrigalWeb.egg-info/PKG-INFO
+-rw-r--r--   0 brideout   (501) staff       (20)      450 2023-07-31 20:04:21.000000 madrigalWeb-3.2.4/madrigalWeb.egg-info/SOURCES.txt
+-rw-r--r--   0 brideout   (501) staff       (20)        1 2023-07-31 20:04:20.000000 madrigalWeb-3.2.4/madrigalWeb.egg-info/dependency_links.txt
+-rw-r--r--   0 brideout   (501) staff       (20)       12 2023-07-31 20:04:21.000000 madrigalWeb-3.2.4/madrigalWeb.egg-info/top_level.txt
+-rw-r--r--   0 brideout   (501) staff       (20)       38 2023-07-31 20:04:21.000000 madrigalWeb-3.2.4/setup.cfg
+-rw-r--r--   0 brideout   (501) staff       (20)      659 2023-07-31 20:03:39.000000 madrigalWeb-3.2.4/setup.py
```

### Comparing `madrigalWeb-3.2.3/documentation/madrigal.css` & `madrigalWeb-3.2.4/documentation/madrigal.css`

 * *Files identical despite different names*

### Comparing `madrigalWeb-3.2.3/documentation/madrigalWeb.html` & `madrigalWeb-3.2.4/documentation/madrigalWeb.html`

 * *Files identical despite different names*

### Comparing `madrigalWeb-3.2.3/documentation/python_scripts.html` & `madrigalWeb-3.2.4/documentation/python_scripts.html`

 * *Files identical despite different names*

### Comparing `madrigalWeb-3.2.3/madrigalWeb/examples/exampleMadrigalWebServices.py` & `madrigalWeb-3.2.4/madrigalWeb/examples/exampleMadrigalWebServices.py`

 * *Files identical despite different names*

### Comparing `madrigalWeb-3.2.3/madrigalWeb/globalCitation.py` & `madrigalWeb-3.2.4/madrigalWeb/globalCitation.py`

 * *Files identical despite different names*

### Comparing `madrigalWeb-3.2.3/madrigalWeb/globalDownload.py` & `madrigalWeb-3.2.4/madrigalWeb/globalDownload.py`

 * *Files identical despite different names*

### Comparing `madrigalWeb-3.2.3/madrigalWeb/globalIsprint.py` & `madrigalWeb-3.2.4/madrigalWeb/globalIsprint.py`

 * *Files identical despite different names*

### Comparing `madrigalWeb-3.2.3/madrigalWeb/madrigalWeb.py` & `madrigalWeb-3.2.4/madrigalWeb/madrigalWeb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """The madrigalWeb module provides access to all Madrigal data via web services.
 
 """
 
-# $Id: madrigalWeb.py 7473 2022-11-08 21:25:02Z brideout $
+# $Id: madrigalWeb.py 7563 2023-07-31 20:03:10Z brideout $
 
 
 import os, os.path, sys
 import traceback
 try:                        # Python 3
     import urllib.request as urllib2
     import urllib.parse as urlparse
 except ImportError:         # Python 2
     import urllib, urllib2, urlparse
 import types
 import re
 import datetime
-import distutils.version
+import packaging.version
 
 # constants
 TIMEOUT = 60 * 30 # timeout in seconds before skipping file
 TIMEOUT2 = 60 * 3 # shorter time out
 
 def isStringType(input):
     """isStringType is a method designed to work with both python 2 and 3 to test for string type
@@ -95,25 +95,24 @@
             raise ValueError('invalid url: ' + str(url))
 
         result = result.group()
         
         if type(result) in (list, tuple):
             result = result[0]
             
-        self.cgiurl = urlBase + result[1:(-1*len(cgiName))]
-
-        try:
-            self.siteDict = self.__getSiteDict()
-        except:
+        if len(result[1:(-1*len(cgiName))]) < 2:
             self.cgiurl = url
-            if not self.cgiurl[-1] == '/':
-                self.cgiurl += '/'
-            self.siteDict = self.__getSiteDict()
+        else:
+            self.cgiurl = urlBase + result[1:(-1*len(cgiName))]
             
+        if not self.cgiurl[-1] == '/':
+                self.cgiurl += '/'
 
+        self.siteDict = self.__getSiteDict()
+            
         self.siteId = self.__getSiteId()
         
         # get Madrigal version
         self._madVers = self.getVersion()
 
 
     def __getSiteDict(self):
@@ -630,16 +629,17 @@
         url = self.cgiurl + scriptName + '?'
 
         
         url += 'file=%s&' % (filename.replace('/', '%2F'))
         if parms.find(' ') != -1:
             parms = parms.replace(' ', '') # remove all spaces
         parms = parms.replace('+','%2B')
-        parms = parms.replace(',','+')
-        url += 'parms=%s&' % (parms)
+        parms = parms.split(',')
+        for p in parms:
+            url += 'parms=%s&' % (p)
         filters = filters.replace('=','%3D')
         filters = filters.replace(',','%2C')
         filters = filters.replace('/','%2F')
         filters = filters.replace('+','%2B')
         filters = filters.replace(' ','+')
         url += 'filters=%s&' % (filters)
         user_fullname = user_fullname.replace(' ','+').strip()
@@ -656,15 +656,15 @@
             elif file_extension in ('.nc',):
                 format = 'netCDF4'
             else:
                 format = 'ascii'
             # if Hdf5 or netCDF4, make sure site is 3 or greater
             if format in ('Hdf5', 'netCDF4'):
                 version = self.getVersion()
-                if distutils.version.LooseVersion(version) < distutils.version.LooseVersion('3.0'):
+                if packaging.version.parse(version) < packaging.version.parse('3.0'):
                     raise ValueError('Madrigal site at %s is below 3.0, cannot convert to Hdf5 or netCDF4' % (self.cgiurl))
         else:
             format = 'ascii'
 
         # read main url
         url = url.replace('+', '%2B')
         try:
@@ -2020,15 +2020,15 @@
     
     
     def compareVersions(self, ver1, ver2):
         """compareVersions returns False if ver1 <= ver2, 0 True otherwise
         
         Inputs: version number strings, in form number dot number (any number of dots)
         """
-        return(distutils.version.LooseVersion(ver1) > distutils.version.LooseVersion(ver2))
+        return(packaging.version.parse(ver1) > packaging.version.parse(ver2))
             
 
     def getCitedFilesFromUrl(self, url):
         """getCitedFilesFromUrl returns a list of citations to individual Madrigal file from a group id url
         as found in a publication
         """
         # read main url
```

### Comparing `madrigalWeb-3.2.3/setup.py` & `madrigalWeb-3.2.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """set up file for the Python Madrigal Remote API
 
-$Id: setup.py 7472 2022-11-08 21:23:40Z brideout $
+$Id: setup.py 7564 2023-07-31 20:03:39Z brideout $
 """
 import os, os.path, sys
 
 from distutils.core import setup
     
 setup(name="madrigalWeb",
-      version="3.2.3",
+      version="3.2.4",
       description="Remote Madrigal Python API",
       author="Bill Rideout",
       author_email="brideout@haystack.mit.edu",
       url="http://cedar.openmadrigal.org",
       packages=["madrigalWeb"],
       keywords = ['Madrigal'],
       scripts=['madrigalWeb/globalIsprint.py', 'madrigalWeb/globalDownload.py',
```

