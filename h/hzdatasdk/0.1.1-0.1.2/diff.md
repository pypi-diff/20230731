# Comparing `tmp/hzdatasdk-0.1.1.tar.gz` & `tmp/hzdatasdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\goProject\xuangu\branches\hzdata\pysvrs\packaging_tutorial\dist\.tmp-rpicfbny\hzdatasdk-0.1.1.tar", last modified: Wed Jan  4 02:30:10 2023, max compression
+gzip compressed data, was "hzdatasdk-0.1.2.tar", last modified: Mon Jul 31 09:18:12 2023, max compression
```

## Comparing `hzdatasdk-0.1.1.tar` & `hzdatasdk-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-01-04 02:30:10.836749 hzdatasdk-0.1.1/
--rw-rw-rw-   0        0        0     1091 2022-11-07 05:23:49.000000 hzdatasdk-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1304 2023-01-04 02:30:10.836749 hzdatasdk-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      802 2023-01-04 02:27:16.000000 hzdatasdk-0.1.1/README.md
--rw-rw-rw-   0        0        0      109 2022-11-07 05:23:49.000000 hzdatasdk-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      714 2023-01-04 02:30:10.836749 hzdatasdk-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-04 02:30:10.719210 hzdatasdk-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-01-04 02:30:10.804652 hzdatasdk-0.1.1/src/hzdatasdk/
--rw-rw-rw-   0        0        0      346 2022-11-07 05:23:49.000000 hzdatasdk-0.1.1/src/hzdatasdk/__init__.py
--rw-rw-rw-   0        0        0     5386 2022-12-30 03:28:15.000000 hzdatasdk-0.1.1/src/hzdatasdk/api.py
--rw-rw-rw-   0        0        0    71706 2022-11-07 05:23:49.000000 hzdatasdk-0.1.1/src/hzdatasdk/choice.py
--rw-rw-rw-   0        0        0     8695 2022-11-07 05:23:49.000000 hzdatasdk-0.1.1/src/hzdatasdk/choiceinfo.py
--rw-rw-rw-   0        0        0     3174 2022-11-07 05:23:49.000000 hzdatasdk-0.1.1/src/hzdatasdk/client.py
--rw-rw-rw-   0        0        0     3484 2022-11-07 05:23:49.000000 hzdatasdk-0.1.1/src/hzdatasdk/hz_finance_service.py
--rw-rw-rw-   0        0        0     5371 2022-11-07 05:23:49.000000 hzdatasdk-0.1.1/src/hzdatasdk/hzdata_pb2.py
--rw-rw-rw-   0        0        0     2413 2022-11-07 05:23:49.000000 hzdatasdk-0.1.1/src/hzdatasdk/hzdata_pb2_grpc.py
--rw-rw-rw-   0        0        0    10697 2022-11-07 05:23:49.000000 hzdatasdk-0.1.1/src/hzdatasdk/utils.py
-drwxrwxrwx   0        0        0        0 2023-01-04 02:30:10.836749 hzdatasdk-0.1.1/src/hzdatasdk.egg-info/
--rw-rw-rw-   0        0        0     1304 2023-01-04 02:30:10.000000 hzdatasdk-0.1.1/src/hzdatasdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      469 2023-01-04 02:30:10.000000 hzdatasdk-0.1.1/src/hzdatasdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-04 02:30:10.000000 hzdatasdk-0.1.1/src/hzdatasdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-01-04 02:30:10.000000 hzdatasdk-0.1.1/src/hzdatasdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-01-04 02:30:10.000000 hzdatasdk-0.1.1/src/hzdatasdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 09:18:12.671119 hzdatasdk-0.1.2/
+-rw-rw-rw-   0        0        0     1091 2022-06-09 02:32:27.000000 hzdatasdk-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1304 2023-07-31 09:18:12.672119 hzdatasdk-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      802 2023-01-18 01:06:13.000000 hzdatasdk-0.1.2/README.md
+-rw-rw-rw-   0        0        0      109 2022-06-09 02:32:27.000000 hzdatasdk-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      714 2023-07-31 09:18:12.675118 hzdatasdk-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 09:18:12.298118 hzdatasdk-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 09:18:12.547118 hzdatasdk-0.1.2/src/hzdatasdk/
+-rw-rw-rw-   0        0        0      346 2022-06-09 02:32:27.000000 hzdatasdk-0.1.2/src/hzdatasdk/__init__.py
+-rw-rw-rw-   0        0        0     6186 2023-07-31 08:05:22.000000 hzdatasdk-0.1.2/src/hzdatasdk/api.py
+-rw-rw-rw-   0        0        0    71706 2022-06-09 02:32:27.000000 hzdatasdk-0.1.2/src/hzdatasdk/choice.py
+-rw-rw-rw-   0        0        0     8695 2022-06-09 02:32:27.000000 hzdatasdk-0.1.2/src/hzdatasdk/choiceinfo.py
+-rw-rw-rw-   0        0        0     3174 2022-10-21 02:12:54.000000 hzdatasdk-0.1.2/src/hzdatasdk/client.py
+-rw-rw-rw-   0        0        0     3484 2022-06-09 02:32:27.000000 hzdatasdk-0.1.2/src/hzdatasdk/hz_finance_service.py
+-rw-rw-rw-   0        0        0     5371 2022-06-09 02:32:27.000000 hzdatasdk-0.1.2/src/hzdatasdk/hzdata_pb2.py
+-rw-rw-rw-   0        0        0     2413 2022-06-09 02:32:27.000000 hzdatasdk-0.1.2/src/hzdatasdk/hzdata_pb2_grpc.py
+-rw-rw-rw-   0        0        0    10697 2022-06-09 02:32:27.000000 hzdatasdk-0.1.2/src/hzdatasdk/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 09:18:12.630117 hzdatasdk-0.1.2/src/hzdatasdk.egg-info/
+-rw-rw-rw-   0        0        0     1304 2023-07-31 09:18:12.000000 hzdatasdk-0.1.2/src/hzdatasdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2023-07-31 09:18:12.000000 hzdatasdk-0.1.2/src/hzdatasdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 09:18:12.000000 hzdatasdk-0.1.2/src/hzdatasdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-07-31 09:18:12.000000 hzdatasdk-0.1.2/src/hzdatasdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-31 09:18:12.000000 hzdatasdk-0.1.2/src/hzdatasdk.egg-info/top_level.txt
```

### Comparing `hzdatasdk-0.1.1/LICENSE` & `hzdatasdk-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hzdatasdk-0.1.1/PKG-INFO` & `hzdatasdk-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: hzdatasdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: shanghai hz finance data sdk
 Home-page: https://github.com/pypa/hzdatasdk
 Author: hz finance
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/pypa/hzdatasdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hzdatasdk Package
 
 This is a simple example package. You can use
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
```

### Comparing `hzdatasdk-0.1.1/README.md` & `hzdatasdk-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `hzdatasdk-0.1.1/setup.cfg` & `hzdatasdk-0.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2068 7a64 6174 6173 646b 0d0a 7665   = hzdatasdk..ve
-00000020: 7273 696f 6e20 3d20 302e 312e 310d 0a61  rsion = 0.1.1..a
+00000020: 7273 696f 6e20 3d20 302e 312e 320d 0a61  rsion = 0.1.2..a
 00000030: 7574 686f 7220 3d20 687a 2066 696e 616e  uthor = hz finan
 00000040: 6365 0d0a 6175 7468 6f72 5f65 6d61 696c  ce..author_email
 00000050: 203d 2061 7574 686f 7240 6578 616d 706c   = author@exampl
 00000060: 652e 636f 6d0d 0a64 6573 6372 6970 7469  e.com..descripti
 00000070: 6f6e 203d 2073 6861 6e67 6861 6920 687a  on = shanghai hz
 00000080: 2066 696e 616e 6365 2064 6174 6120 7364   finance data sd
 00000090: 6b0d 0a6c 6f6e 675f 6465 7363 7269 7074  k..long_descript
@@ -28,15 +28,15 @@
 000001b0: 6963 656e 7365 0d0a 094f 7065 7261 7469  icense...Operati
 000001c0: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
 000001d0: 496e 6465 7065 6e64 656e 740d 0a0d 0a5b  Independent....[
 000001e0: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
 000001f0: 655f 6469 7220 3d20 0d0a 093d 2073 7263  e_dir = ...= src
 00000200: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
 00000210: 643a 0d0a 7079 7468 6f6e 5f72 6571 7569  d:..python_requi
-00000220: 7265 7320 3d20 3e3d 332e 360d 0a69 6e73  res = >=3.6..ins
+00000220: 7265 7320 3d20 3e3d 332e 370d 0a69 6e73  res = >=3.7..ins
 00000230: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
 00000240: 7369 783b 7061 6e64 6173 3e3d 312e 332e  six;pandas>=1.3.
 00000250: 353b 6d73 6770 6163 6b3b 7371 6c61 6c63  5;msgpack;sqlalc
 00000260: 6865 6d79 3b67 7270 6369 6f3b 7072 6f74  hemy;grpcio;prot
 00000270: 6f62 7566 0d0a 0d0a 5b6f 7074 696f 6e73  obuf....[options
 00000280: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
 00000290: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
```

### Comparing `hzdatasdk-0.1.1/src/hzdatasdk/api.py` & `hzdatasdk-0.1.2/src/hzdatasdk/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -107,13 +107,34 @@
     end_date = to_datetime_str(end_date)
     if (not count) and (not start_date):
         start_date = "2015-01-01"
     if count and start_date:
         raise ParamsError("(start_date, count) only one param is required")
     return HZDataClient.instance().get_industry(**locals())
 
+def query_minute_trade(security=None, date=None):
+    if security is None:
+        raise ParamsError("security is required")
+    if date is None:
+        raise ParamsError("date is required")
+    return HZDataClient.instance().get_minute_trade(**locals())
+
+def query_minute_buy_sell1(security=None, date=None):
+    if security is None:
+        raise ParamsError("security is required")
+    if date is None:
+        raise ParamsError("date is required")
+    return HZDataClient.instance().get_minute_buy_sell1(**locals())
+
+def query_minute_kline(security=None, date=None):
+    if security is None:
+        raise ParamsError("security is required")
+    if date is None:
+        raise ParamsError("date is required")
+    return HZDataClient.instance().get_minute_kline(**locals())
+
 
 __all__ = [
     "query"
 ]
 __all__.extend(_collect_func())
 del _collect_func
```

### Comparing `hzdatasdk-0.1.1/src/hzdatasdk/choice.py` & `hzdatasdk-0.1.2/src/hzdatasdk/choice.py`

 * *Files identical despite different names*

### Comparing `hzdatasdk-0.1.1/src/hzdatasdk/choiceinfo.py` & `hzdatasdk-0.1.2/src/hzdatasdk/choiceinfo.py`

 * *Files identical despite different names*

### Comparing `hzdatasdk-0.1.1/src/hzdatasdk/client.py` & `hzdatasdk-0.1.2/src/hzdatasdk/client.py`

 * *Files identical despite different names*

### Comparing `hzdatasdk-0.1.1/src/hzdatasdk/hz_finance_service.py` & `hzdatasdk-0.1.2/src/hzdatasdk/hz_finance_service.py`

 * *Files identical despite different names*

### Comparing `hzdatasdk-0.1.1/src/hzdatasdk/hzdata_pb2.py` & `hzdatasdk-0.1.2/src/hzdatasdk/hzdata_pb2.py`

 * *Files identical despite different names*

### Comparing `hzdatasdk-0.1.1/src/hzdatasdk/hzdata_pb2_grpc.py` & `hzdatasdk-0.1.2/src/hzdatasdk/hzdata_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hzdatasdk-0.1.1/src/hzdatasdk/utils.py` & `hzdatasdk-0.1.2/src/hzdatasdk/utils.py`

 * *Files identical despite different names*

### Comparing `hzdatasdk-0.1.1/src/hzdatasdk.egg-info/PKG-INFO` & `hzdatasdk-0.1.2/src/hzdatasdk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: hzdatasdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: shanghai hz finance data sdk
 Home-page: https://github.com/pypa/hzdatasdk
 Author: hz finance
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/pypa/hzdatasdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hzdatasdk Package
 
 This is a simple example package. You can use
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
```

