# Comparing `tmp/geodatacrawler-0.1.1.tar.gz` & `tmp/geodatacrawler-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geodatacrawler-0.1.1.tar", max compression
+gzip compressed data, was "geodatacrawler-0.1.2.tar", max compression
```

## Comparing `geodatacrawler-0.1.1.tar` & `geodatacrawler-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rwxr-xr-x   0        0        0     1096 2023-06-20 07:37:01.011896 geodatacrawler-0.1.1/LICENSE
--rwxr-xr-x   0        0        0       23 2023-06-20 07:37:01.153896 geodatacrawler-0.1.1/geodatacrawler/__init__.py
--rwxr-xr-x   0        0        0      220 2023-06-20 07:37:01.153896 geodatacrawler-0.1.1/geodatacrawler/etl.py
--rwxr-xr-x   0        0        0    16594 2023-06-20 07:37:01.154895 geodatacrawler-0.1.1/geodatacrawler/mapfile.py
--rwxr-xr-x   0        0        0    30096 2023-07-06 08:48:38.498475 geodatacrawler-0.1.1/geodatacrawler/metadata.py
--rwxr-xr-x   0        0        0     7379 2023-06-20 07:37:01.156897 geodatacrawler-0.1.1/geodatacrawler/schemas/iso19139/__init__.py
--rwxr-xr-x   0        0        0     3603 2023-06-22 07:00:12.939812 geodatacrawler-0.1.1/geodatacrawler/schemas/iso19139/contact.j2
--rwxr-xr-x   0        0        0    21854 2023-06-22 07:00:12.941435 geodatacrawler-0.1.1/geodatacrawler/schemas/iso19139/main.j2
--rwxr-xr-x   0        0        0      307 2023-07-06 08:28:47.933795 geodatacrawler-0.1.1/geodatacrawler/templates/PGM.tpl
--rwxr-xr-x   0        0        0       21 2023-06-20 07:37:01.159894 geodatacrawler-0.1.1/geodatacrawler/templates/__init__.py
--rwxr-xr-x   0        0        0      118 2023-06-20 07:37:01.160911 geodatacrawler-0.1.1/geodatacrawler/templates/class-line.tpl
--rwxr-xr-x   0        0        0      118 2023-06-20 07:37:01.161895 geodatacrawler-0.1.1/geodatacrawler/templates/class-point.tpl
--rwxr-xr-x   0        0        0      137 2023-06-20 07:37:01.161895 geodatacrawler-0.1.1/geodatacrawler/templates/class-polygon.tpl
--rwxr-xr-x   0        0        0     6622 2023-06-20 07:37:01.162898 geodatacrawler-0.1.1/geodatacrawler/templates/class-raster.tpl
--rwxr-xr-x   0        0        0     2112 2023-06-20 07:37:01.163900 geodatacrawler-0.1.1/geodatacrawler/templates/csv.j2
--rwxr-xr-x   0        0        0     2860 2023-06-20 07:37:01.164899 geodatacrawler-0.1.1/geodatacrawler/templates/default.map
--rwxr-xr-x   0        0        0    12288 2023-06-20 07:37:01.164899 geodatacrawler-0.1.1/geodatacrawler/templates/index.sqlite
--rwxr-xr-x   0        0        0      722 2023-06-20 07:37:01.165896 geodatacrawler-0.1.1/geodatacrawler/templates/layer.tpl
--rwxr-xr-x   0        0        0     6686 2023-06-20 07:37:01.166897 geodatacrawler-0.1.1/geodatacrawler/upload.py
--rwxr-xr-x   0        0        0    17081 2023-06-20 07:37:01.167895 geodatacrawler-0.1.1/geodatacrawler/upload_wosis.py
--rwxr-xr-x   0        0        0    21760 2023-07-04 11:48:26.220044 geodatacrawler-0.1.1/geodatacrawler/utils.py
--rwxr-xr-x   0        0        0     1009 2023-07-31 12:25:02.296828 geodatacrawler-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1184 1970-01-01 00:00:00.000000 geodatacrawler-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1096 2023-06-20 07:37:01.011896 geodatacrawler-0.1.2/LICENSE
+-rwxr-xr-x   0        0        0     5036 2023-06-22 07:00:12.921422 geodatacrawler-0.1.2/README.md
+-rwxr-xr-x   0        0        0       23 2023-06-20 07:37:01.153896 geodatacrawler-0.1.2/geodatacrawler/__init__.py
+-rwxr-xr-x   0        0        0      220 2023-06-20 07:37:01.153896 geodatacrawler-0.1.2/geodatacrawler/etl.py
+-rwxr-xr-x   0        0        0    16594 2023-06-20 07:37:01.154895 geodatacrawler-0.1.2/geodatacrawler/mapfile.py
+-rwxr-xr-x   0        0        0    30096 2023-07-06 08:48:38.498475 geodatacrawler-0.1.2/geodatacrawler/metadata.py
+-rwxr-xr-x   0        0        0     7379 2023-06-20 07:37:01.156897 geodatacrawler-0.1.2/geodatacrawler/schemas/iso19139/__init__.py
+-rwxr-xr-x   0        0        0     3603 2023-06-22 07:00:12.939812 geodatacrawler-0.1.2/geodatacrawler/schemas/iso19139/contact.j2
+-rwxr-xr-x   0        0        0    21854 2023-06-22 07:00:12.941435 geodatacrawler-0.1.2/geodatacrawler/schemas/iso19139/main.j2
+-rwxr-xr-x   0        0        0      307 2023-07-06 08:28:47.933795 geodatacrawler-0.1.2/geodatacrawler/templates/PGM.tpl
+-rwxr-xr-x   0        0        0       21 2023-06-20 07:37:01.159894 geodatacrawler-0.1.2/geodatacrawler/templates/__init__.py
+-rwxr-xr-x   0        0        0      118 2023-06-20 07:37:01.160911 geodatacrawler-0.1.2/geodatacrawler/templates/class-line.tpl
+-rwxr-xr-x   0        0        0      118 2023-06-20 07:37:01.161895 geodatacrawler-0.1.2/geodatacrawler/templates/class-point.tpl
+-rwxr-xr-x   0        0        0      137 2023-06-20 07:37:01.161895 geodatacrawler-0.1.2/geodatacrawler/templates/class-polygon.tpl
+-rwxr-xr-x   0        0        0     6622 2023-06-20 07:37:01.162898 geodatacrawler-0.1.2/geodatacrawler/templates/class-raster.tpl
+-rwxr-xr-x   0        0        0     2112 2023-06-20 07:37:01.163900 geodatacrawler-0.1.2/geodatacrawler/templates/csv.j2
+-rwxr-xr-x   0        0        0     2860 2023-06-20 07:37:01.164899 geodatacrawler-0.1.2/geodatacrawler/templates/default.map
+-rwxr-xr-x   0        0        0    12288 2023-06-20 07:37:01.164899 geodatacrawler-0.1.2/geodatacrawler/templates/index.sqlite
+-rwxr-xr-x   0        0        0      722 2023-06-20 07:37:01.165896 geodatacrawler-0.1.2/geodatacrawler/templates/layer.tpl
+-rwxr-xr-x   0        0        0     6686 2023-06-20 07:37:01.166897 geodatacrawler-0.1.2/geodatacrawler/upload.py
+-rwxr-xr-x   0        0        0    17081 2023-06-20 07:37:01.167895 geodatacrawler-0.1.2/geodatacrawler/upload_wosis.py
+-rwxr-xr-x   0        0        0    21760 2023-07-04 11:48:26.220044 geodatacrawler-0.1.2/geodatacrawler/utils.py
+-rwxr-xr-x   0        0        0     1031 2023-07-31 12:33:42.239832 geodatacrawler-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6133 1970-01-01 00:00:00.000000 geodatacrawler-0.1.2/PKG-INFO
```

### Comparing `geodatacrawler-0.1.1/LICENSE` & `geodatacrawler-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.1/geodatacrawler/mapfile.py` & `geodatacrawler-0.1.2/geodatacrawler/mapfile.py`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.1/geodatacrawler/metadata.py` & `geodatacrawler-0.1.2/geodatacrawler/metadata.py`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.1/geodatacrawler/schemas/iso19139/__init__.py` & `geodatacrawler-0.1.2/geodatacrawler/schemas/iso19139/__init__.py`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.1/geodatacrawler/schemas/iso19139/contact.j2` & `geodatacrawler-0.1.2/geodatacrawler/schemas/iso19139/contact.j2`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.1/geodatacrawler/schemas/iso19139/main.j2` & `geodatacrawler-0.1.2/geodatacrawler/schemas/iso19139/main.j2`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.1/geodatacrawler/templates/class-raster.tpl` & `geodatacrawler-0.1.2/geodatacrawler/templates/class-raster.tpl`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.1/geodatacrawler/templates/csv.j2` & `geodatacrawler-0.1.2/geodatacrawler/templates/csv.j2`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.1/geodatacrawler/templates/default.map` & `geodatacrawler-0.1.2/geodatacrawler/templates/default.map`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.1/geodatacrawler/templates/index.sqlite` & `geodatacrawler-0.1.2/geodatacrawler/templates/index.sqlite`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.1/geodatacrawler/templates/layer.tpl` & `geodatacrawler-0.1.2/geodatacrawler/templates/layer.tpl`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.1/geodatacrawler/upload.py` & `geodatacrawler-0.1.2/geodatacrawler/upload.py`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.1/geodatacrawler/upload_wosis.py` & `geodatacrawler-0.1.2/geodatacrawler/upload_wosis.py`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.1/geodatacrawler/utils.py` & `geodatacrawler-0.1.2/geodatacrawler/utils.py`

 * *Files identical despite different names*

### Comparing `geodatacrawler-0.1.1/pyproject.toml` & `geodatacrawler-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "geodatacrawler"
-version = "0.1.1"
+version = "0.1.2"
 license = "MIT"
 description = "a crawler script to extract and author metadata of spatial datasets"
 authors = ["Paul van Genuchten <genuchten@yahoo.com>"]
+readme = "README.md"
 repository = "https://github.com/pvgenuchten/pyGeoDataCrawler"
 packages = [
     { include = "geodatacrawler" },
     { include = "geodatacrawler/templates/*" },
 ]
 
 [tool.poetry.dependencies]
```

