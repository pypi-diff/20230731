# Comparing `tmp/geodatacrawler-1.1.0.tar.gz` & `tmp/geodatacrawler-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geodatacrawler-1.1.0.tar", max compression
+gzip compressed data, was "geodatacrawler-1.1.1.tar", max compression
```

## Comparing `geodatacrawler-1.1.0.tar` & `geodatacrawler-1.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rwxr-xr-x   0        0        0     1096 2023-06-20 07:37:01.011896 geodatacrawler-1.1.0/LICENSE
--rwxr-xr-x   0        0        0     3756 2023-07-31 14:47:49.815210 geodatacrawler-1.1.0/README.md
--rwxr-xr-x   0        0        0       23 2023-06-20 07:37:01.153896 geodatacrawler-1.1.0/geodatacrawler/__init__.py
--rwxr-xr-x   0        0        0      220 2023-06-20 07:37:01.153896 geodatacrawler-1.1.0/geodatacrawler/etl.py
--rwxr-xr-x   0        0        0    16594 2023-06-20 07:37:01.154895 geodatacrawler-1.1.0/geodatacrawler/mapfile.py
--rwxr-xr-x   0        0        0    30113 2023-07-31 14:47:41.294665 geodatacrawler-1.1.0/geodatacrawler/metadata.py
--rwxr-xr-x   0        0        0     7379 2023-06-20 07:37:01.156897 geodatacrawler-1.1.0/geodatacrawler/schemas/iso19139/__init__.py
--rwxr-xr-x   0        0        0     3603 2023-07-31 12:57:52.922404 geodatacrawler-1.1.0/geodatacrawler/schemas/iso19139/contact.j2
--rwxr-xr-x   0        0        0    21854 2023-07-31 12:57:52.930840 geodatacrawler-1.1.0/geodatacrawler/schemas/iso19139/main.j2
--rwxr-xr-x   0        0        0      307 2023-07-31 12:57:52.942960 geodatacrawler-1.1.0/geodatacrawler/templates/PGM.tpl
--rwxr-xr-x   0        0        0       21 2023-06-20 07:37:01.159894 geodatacrawler-1.1.0/geodatacrawler/templates/__init__.py
--rwxr-xr-x   0        0        0      118 2023-06-20 07:37:01.160911 geodatacrawler-1.1.0/geodatacrawler/templates/class-line.tpl
--rwxr-xr-x   0        0        0      118 2023-06-20 07:37:01.161895 geodatacrawler-1.1.0/geodatacrawler/templates/class-point.tpl
--rwxr-xr-x   0        0        0      137 2023-06-20 07:37:01.161895 geodatacrawler-1.1.0/geodatacrawler/templates/class-polygon.tpl
--rwxr-xr-x   0        0        0     6622 2023-06-20 07:37:01.162898 geodatacrawler-1.1.0/geodatacrawler/templates/class-raster.tpl
--rwxr-xr-x   0        0        0     2112 2023-06-20 07:37:01.163900 geodatacrawler-1.1.0/geodatacrawler/templates/csv.j2
--rwxr-xr-x   0        0        0     2860 2023-06-20 07:37:01.164899 geodatacrawler-1.1.0/geodatacrawler/templates/default.map
--rwxr-xr-x   0        0        0    12288 2023-06-20 07:37:01.164899 geodatacrawler-1.1.0/geodatacrawler/templates/index.sqlite
--rwxr-xr-x   0        0        0      722 2023-06-20 07:37:01.165896 geodatacrawler-1.1.0/geodatacrawler/templates/layer.tpl
--rwxr-xr-x   0        0        0     6686 2023-06-20 07:37:01.166897 geodatacrawler-1.1.0/geodatacrawler/upload.py
--rwxr-xr-x   0        0        0    17081 2023-06-20 07:37:01.167895 geodatacrawler-1.1.0/geodatacrawler/upload_wosis.py
--rwxr-xr-x   0        0        0    21760 2023-07-31 12:57:52.959935 geodatacrawler-1.1.0/geodatacrawler/utils.py
--rwxr-xr-x   0        0        0     1031 2023-07-31 14:48:01.437700 geodatacrawler-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4890 1970-01-01 00:00:00.000000 geodatacrawler-1.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1096 2023-06-20 07:37:01.011896 geodatacrawler-1.1.1/LICENSE
+-rwxr-xr-x   0        0        0     3756 2023-07-31 14:47:49.815210 geodatacrawler-1.1.1/README.md
+-rwxr-xr-x   0        0        0       23 2023-06-20 07:37:01.153896 geodatacrawler-1.1.1/geodatacrawler/__init__.py
+-rwxr-xr-x   0        0        0      220 2023-06-20 07:37:01.153896 geodatacrawler-1.1.1/geodatacrawler/etl.py
+-rwxr-xr-x   0        0        0    16594 2023-06-20 07:37:01.154895 geodatacrawler-1.1.1/geodatacrawler/mapfile.py
+-rwxr-xr-x   0        0        0    30264 2023-07-31 15:02:18.986787 geodatacrawler-1.1.1/geodatacrawler/metadata.py
+-rwxr-xr-x   0        0        0     7379 2023-06-20 07:37:01.156897 geodatacrawler-1.1.1/geodatacrawler/schemas/iso19139/__init__.py
+-rwxr-xr-x   0        0        0     3603 2023-07-31 12:57:52.922404 geodatacrawler-1.1.1/geodatacrawler/schemas/iso19139/contact.j2
+-rwxr-xr-x   0        0        0    21854 2023-07-31 12:57:52.930840 geodatacrawler-1.1.1/geodatacrawler/schemas/iso19139/main.j2
+-rwxr-xr-x   0        0        0      307 2023-07-31 12:57:52.942960 geodatacrawler-1.1.1/geodatacrawler/templates/PGM.tpl
+-rwxr-xr-x   0        0        0       21 2023-06-20 07:37:01.159894 geodatacrawler-1.1.1/geodatacrawler/templates/__init__.py
+-rwxr-xr-x   0        0        0      118 2023-06-20 07:37:01.160911 geodatacrawler-1.1.1/geodatacrawler/templates/class-line.tpl
+-rwxr-xr-x   0        0        0      118 2023-06-20 07:37:01.161895 geodatacrawler-1.1.1/geodatacrawler/templates/class-point.tpl
+-rwxr-xr-x   0        0        0      137 2023-06-20 07:37:01.161895 geodatacrawler-1.1.1/geodatacrawler/templates/class-polygon.tpl
+-rwxr-xr-x   0        0        0     6622 2023-06-20 07:37:01.162898 geodatacrawler-1.1.1/geodatacrawler/templates/class-raster.tpl
+-rwxr-xr-x   0        0        0     2112 2023-06-20 07:37:01.163900 geodatacrawler-1.1.1/geodatacrawler/templates/csv.j2
+-rwxr-xr-x   0        0        0     2860 2023-06-20 07:37:01.164899 geodatacrawler-1.1.1/geodatacrawler/templates/default.map
+-rwxr-xr-x   0        0        0    12288 2023-06-20 07:37:01.164899 geodatacrawler-1.1.1/geodatacrawler/templates/index.sqlite
+-rwxr-xr-x   0        0        0      722 2023-06-20 07:37:01.165896 geodatacrawler-1.1.1/geodatacrawler/templates/layer.tpl
+-rwxr-xr-x   0        0        0     6686 2023-06-20 07:37:01.166897 geodatacrawler-1.1.1/geodatacrawler/upload.py
+-rwxr-xr-x   0        0        0    17081 2023-06-20 07:37:01.167895 geodatacrawler-1.1.1/geodatacrawler/upload_wosis.py
+-rwxr-xr-x   0        0        0    21760 2023-07-31 12:57:52.959935 geodatacrawler-1.1.1/geodatacrawler/utils.py
+-rwxr-xr-x   0        0        0     1031 2023-07-31 15:03:15.148183 geodatacrawler-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4890 1970-01-01 00:00:00.000000 geodatacrawler-1.1.1/PKG-INFO
```

### Comparing `geodatacrawler-1.1.0/LICENSE` & `geodatacrawler-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.0/README.md` & `geodatacrawler-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.0/geodatacrawler/mapfile.py` & `geodatacrawler-1.1.1/geodatacrawler/mapfile.py`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.0/geodatacrawler/metadata.py` & `geodatacrawler-1.1.1/geodatacrawler/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -504,15 +504,19 @@
                 dict_merge(coreMetadata, pathMetadata)
             return coreMetadata
     else:
         return coreMetadata
 
 def load_default_metadata(mode):
     initial = merge_folder_metadata({},'.',mode)
+    if not 'identification' in initial:
+        initial['identification'] = {}
     initial['identification']['dates'] = {"publication": datetime.date.today()}
+    if not 'metadata' in initial:
+        initial['metadata'] = {} 
     initial['metadata']['datestamp'] = datetime.date.today()
     return initial
 
 def createIndexIfDoesntExist(db):
     if path.exists(db):
         print('database ' + db + ' exists')
     else:
```

### Comparing `geodatacrawler-1.1.0/geodatacrawler/schemas/iso19139/__init__.py` & `geodatacrawler-1.1.1/geodatacrawler/schemas/iso19139/__init__.py`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.0/geodatacrawler/schemas/iso19139/contact.j2` & `geodatacrawler-1.1.1/geodatacrawler/schemas/iso19139/contact.j2`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.0/geodatacrawler/schemas/iso19139/main.j2` & `geodatacrawler-1.1.1/geodatacrawler/schemas/iso19139/main.j2`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.0/geodatacrawler/templates/class-raster.tpl` & `geodatacrawler-1.1.1/geodatacrawler/templates/class-raster.tpl`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.0/geodatacrawler/templates/csv.j2` & `geodatacrawler-1.1.1/geodatacrawler/templates/csv.j2`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.0/geodatacrawler/templates/default.map` & `geodatacrawler-1.1.1/geodatacrawler/templates/default.map`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.0/geodatacrawler/templates/index.sqlite` & `geodatacrawler-1.1.1/geodatacrawler/templates/index.sqlite`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.0/geodatacrawler/templates/layer.tpl` & `geodatacrawler-1.1.1/geodatacrawler/templates/layer.tpl`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.0/geodatacrawler/upload.py` & `geodatacrawler-1.1.1/geodatacrawler/upload.py`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.0/geodatacrawler/upload_wosis.py` & `geodatacrawler-1.1.1/geodatacrawler/upload_wosis.py`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.0/geodatacrawler/utils.py` & `geodatacrawler-1.1.1/geodatacrawler/utils.py`

 * *Files identical despite different names*

### Comparing `geodatacrawler-1.1.0/pyproject.toml` & `geodatacrawler-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geodatacrawler"
-version = "1.1.0"
+version = "1.1.1"
 license = "MIT"
 description = "a crawler script to extract and author metadata of spatial datasets"
 authors = ["Paul van Genuchten <genuchten@yahoo.com>"]
 readme = "README.md"
 repository = "https://github.com/pvgenuchten/pyGeoDataCrawler"
 packages = [
     { include = "geodatacrawler" },
```

### Comparing `geodatacrawler-1.1.0/PKG-INFO` & `geodatacrawler-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodatacrawler
-Version: 1.1.0
+Version: 1.1.1
 Summary: a crawler script to extract and author metadata of spatial datasets
 Home-page: https://github.com/pvgenuchten/pyGeoDataCrawler
 License: MIT
 Author: Paul van Genuchten
 Author-email: genuchten@yahoo.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

