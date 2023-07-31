# Comparing `tmp/odoo_addons_shopinvader_odoo_shopinvader-16.0.20230629.0-py3-none-any.whl.zip` & `tmp/odoo_addons_shopinvader_odoo_shopinvader-16.0.20230730.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1516 bytes, number of entries: 4
--rw-r--r--  2.0 unx      546 b- defN 23-Jun-30 02:38 odoo_addons_shopinvader_odoo_shopinvader-16.0.20230629.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 02:38 odoo_addons_shopinvader_odoo_shopinvader-16.0.20230629.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-30 02:38 odoo_addons_shopinvader_odoo_shopinvader-16.0.20230629.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      468 b- defN 23-Jun-30 02:38 odoo_addons_shopinvader_odoo_shopinvader-16.0.20230629.0.dist-info/RECORD
-4 files, 1107 bytes uncompressed, 590 bytes compressed:  46.7%
+Zip file size: 1528 bytes, number of entries: 4
+-rw-r--r--  2.0 unx      758 b- defN 23-Jul-31 02:35 odoo_addons_shopinvader_odoo_shopinvader-16.0.20230730.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-31 02:35 odoo_addons_shopinvader_odoo_shopinvader-16.0.20230730.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-31 02:35 odoo_addons_shopinvader_odoo_shopinvader-16.0.20230730.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      468 b- defN 23-Jul-31 02:35 odoo_addons_shopinvader_odoo_shopinvader-16.0.20230730.0.dist-info/RECORD
+4 files, 1319 bytes uncompressed, 602 bytes compressed:  54.4%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_shopinvader_odoo_shopinvader-16.0.20230629.0.dist-info/METADATA
+Filename: odoo_addons_shopinvader_odoo_shopinvader-16.0.20230730.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_shopinvader_odoo_shopinvader-16.0.20230629.0.dist-info/WHEEL
+Filename: odoo_addons_shopinvader_odoo_shopinvader-16.0.20230730.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_shopinvader_odoo_shopinvader-16.0.20230629.0.dist-info/top_level.txt
+Filename: odoo_addons_shopinvader_odoo_shopinvader-16.0.20230730.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_shopinvader_odoo_shopinvader-16.0.20230629.0.dist-info/RECORD
+Filename: odoo_addons_shopinvader_odoo_shopinvader-16.0.20230730.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_shopinvader_odoo_shopinvader-16.0.20230629.0.dist-info/METADATA` & `odoo_addons_shopinvader_odoo_shopinvader-16.0.20230730.0.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: odoo-addons-shopinvader-odoo-shopinvader
-Version: 16.0.20230629.0
+Version: 16.0.20230730.0
 Summary: Meta package for shopinvader-odoo-shopinvader Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
 Requires-Dist: odoo-addon-sale-cart (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-shopinvader-address (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-shopinvader-anonymous-partner (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-shopinvader-api-address (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-shopinvader-fastapi-auth-jwt (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-shopinvader-schema-address (<16.1dev,>=16.0dev)
 
 UNKNOWN
```

