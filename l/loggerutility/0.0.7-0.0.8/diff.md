# Comparing `tmp/loggerutility-0.0.7-py3-none-any.whl.zip` & `tmp/loggerutility-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3134 bytes, number of entries: 6
--rw-rw-r--  2.0 unx     2043 b- defN 23-Jul-28 13:56 loggerutility/__init__.py
--rw-rw-r--  2.0 unx     1073 b- defN 23-Jul-28 13:58 loggerutility-0.0.7.dist-info/LICENCE.txt
--rw-rw-r--  2.0 unx      527 b- defN 23-Jul-28 13:58 loggerutility-0.0.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-28 13:58 loggerutility-0.0.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Jul-28 13:58 loggerutility-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      501 b- defN 23-Jul-28 13:58 loggerutility-0.0.7.dist-info/RECORD
-6 files, 4250 bytes uncompressed, 2220 bytes compressed:  47.8%
+Zip file size: 3137 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx     2045 b- defN 23-Jul-31 13:44 loggerutility/__init__.py
+-rw-rw-r--  2.0 unx     1073 b- defN 23-Jul-31 13:56 loggerutility-0.0.8.dist-info/LICENCE.txt
+-rw-rw-r--  2.0 unx      527 b- defN 23-Jul-31 13:56 loggerutility-0.0.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-31 13:56 loggerutility-0.0.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-Jul-31 13:56 loggerutility-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      501 b- defN 23-Jul-31 13:56 loggerutility-0.0.8.dist-info/RECORD
+6 files, 4252 bytes uncompressed, 2223 bytes compressed:  47.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: loggerutility/__init__.py
 Comment: 
 
-Filename: loggerutility-0.0.7.dist-info/LICENCE.txt
+Filename: loggerutility-0.0.8.dist-info/LICENCE.txt
 Comment: 
 
-Filename: loggerutility-0.0.7.dist-info/METADATA
+Filename: loggerutility-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: loggerutility-0.0.7.dist-info/WHEEL
+Filename: loggerutility-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: loggerutility-0.0.7.dist-info/top_level.txt
+Filename: loggerutility-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: loggerutility-0.0.7.dist-info/RECORD
+Filename: loggerutility-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## loggerutility/__init__.py

```diff
@@ -48,15 +48,15 @@
                     filemode=filemode,
                     level=logging.DEBUG)
 logger = logging.getLogger(loggerName)
 logHandler = RotatingFileHandler(dir + '/' + filename, maxBytes=int(maxBytes), backupCount=int(backUpcount))
 logger.addHandler(logHandler)
 
 
-def log(msg, debugLevel=0):
+def log(msg, debugLevel='0'):
     stack = traceback.extract_stack()
     filename, line, functionName, text = stack[-2]
     index = filename.rfind('/')
     filename = filename[index + 1:]
     msg = '~' + filename + '~' + functionName + '~' + msg
 
     if debugLevel.strip() == '':
```

## Comparing `loggerutility-0.0.7.dist-info/LICENCE.txt` & `loggerutility-0.0.8.dist-info/LICENCE.txt`

 * *Files identical despite different names*

## Comparing `loggerutility-0.0.7.dist-info/METADATA` & `loggerutility-0.0.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerutility
-Version: 0.0.7
+Version: 0.0.8
 Summary: Proteus Logger File
 Author: Proteus Technology PVT. LTD.
 Author-email: <apps@baseinformation.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

