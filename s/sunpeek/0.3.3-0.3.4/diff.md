# Comparing `tmp/sunpeek-0.3.3-py3-none-any.whl.zip` & `tmp/sunpeek-0.3.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -64,13 +64,13 @@
 -rw-r--r--  2.0 unx     2532 b- defN 80-Jan-01 00:00 sunpeek/definitions/fluid_data/Wocklum Thermum P/heat capacity.csv
 -rw-r--r--  2.0 unx    33003 b- defN 80-Jan-01 00:00 sunpeek/definitions/fluid_definitions.py
 -rw-r--r--  2.0 unx      528 b- defN 80-Jan-01 00:00 sunpeek/demo/__init__.py
 -rw-r--r--  2.0 unx     1902 b- defN 80-Jan-01 00:00 sunpeek/demo/demo_plant.py
 -rw-r--r--  2.0 unx     5168 b- defN 80-Jan-01 00:00 sunpeek/demo/demo_plant_script.py
 -rw-r--r--  2.0 unx     6191 b- defN 80-Jan-01 00:00 sunpeek/exporter.py
 -rw-r--r--  2.0 unx    22210 b- defN 80-Jan-01 00:00 sunpeek/serializable_models.py
--rw-r--r--  2.0 unx     7652 b- defN 80-Jan-01 00:00 sunpeek-0.3.3.dist-info/COPYING.LESSER
--rw-r--r--  2.0 unx    15233 b- defN 80-Jan-01 00:00 sunpeek-0.3.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 sunpeek-0.3.3.dist-info/WHEEL
--rw-r--r--  2.0 unx    35149 b- defN 80-Jan-01 00:00 sunpeek-0.3.3.dist-info/COPYING
-?rw-r--r--  2.0 unx     6727 b- defN 16-Jan-01 00:00 sunpeek-0.3.3.dist-info/RECORD
+-rw-r--r--  2.0 unx     7652 b- defN 80-Jan-01 00:00 sunpeek-0.3.4.dist-info/COPYING.LESSER
+-rw-r--r--  2.0 unx    15233 b- defN 80-Jan-01 00:00 sunpeek-0.3.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 sunpeek-0.3.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx    35149 b- defN 80-Jan-01 00:00 sunpeek-0.3.4.dist-info/COPYING
+?rw-r--r--  2.0 unx     6727 b- defN 16-Jan-01 00:00 sunpeek-0.3.4.dist-info/RECORD
 74 files, 713624 bytes uncompressed, 183099 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -201,23 +201,23 @@
 
 Filename: sunpeek/exporter.py
 Comment: 
 
 Filename: sunpeek/serializable_models.py
 Comment: 
 
-Filename: sunpeek-0.3.3.dist-info/COPYING.LESSER
+Filename: sunpeek-0.3.4.dist-info/COPYING.LESSER
 Comment: 
 
-Filename: sunpeek-0.3.3.dist-info/METADATA
+Filename: sunpeek-0.3.4.dist-info/METADATA
 Comment: 
 
-Filename: sunpeek-0.3.3.dist-info/WHEEL
+Filename: sunpeek-0.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: sunpeek-0.3.3.dist-info/COPYING
+Filename: sunpeek-0.3.4.dist-info/COPYING
 Comment: 
 
-Filename: sunpeek-0.3.3.dist-info/RECORD
+Filename: sunpeek-0.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `sunpeek-0.3.3.dist-info/COPYING.LESSER` & `sunpeek-0.3.4.dist-info/COPYING.LESSER`

 * *Files identical despite different names*

## Comparing `sunpeek-0.3.3.dist-info/METADATA` & `sunpeek-0.3.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunpeek
-Version: 0.3.3
+Version: 0.3.4
 Summary: Large Solar Thermal Monitoring Tool. Implements the Performance Check Method of ISO 24194
 Home-page: https://gitlab.com/sunpeek/sunpeek
 License: LGPL-3.0-only
 Keywords: solarthermal,solar,energy,monitoring
 Author: Philip Ohnewein, Daniel Tschopp, Lukas Feierl, Marnoch Hamilton-Jones, Jonathan Cazco
 Maintainer: Marnoch Hamilton-Jones
 Maintainer-email: m.hamilton-jones@aee.at
```

## Comparing `sunpeek-0.3.3.dist-info/COPYING` & `sunpeek-0.3.4.dist-info/COPYING`

 * *Files identical despite different names*

## Comparing `sunpeek-0.3.3.dist-info/RECORD` & `sunpeek-0.3.4.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -63,12 +63,12 @@
 sunpeek/definitions/fluid_data/Wocklum Thermum P/heat capacity.csv,sha256=F-IZeYyL2U3rww2tTP1qRWH0bCY3FhGY7f9-FtlvZ_w,2532
 sunpeek/definitions/fluid_definitions.py,sha256=Qry_kWr-cHKEnEbKl9WolUiAJ9g2NzO-rnmIVNpJ2lI,33003
 sunpeek/demo/__init__.py,sha256=djMLgvrYODa5bcBr2KnbPZ37s1yO_3igMAEYNXp_iPQ,528
 sunpeek/demo/demo_plant.py,sha256=tVfvaM7wa2bWLIeZxwpykS0HHxPsoxXthU9zfwJV6Gs,1902
 sunpeek/demo/demo_plant_script.py,sha256=ifWIWRvLTA-IYaTfM-BGZc6mnh15A3-SOwFTs2ehKuE,5168
 sunpeek/exporter.py,sha256=okT1A2hiRjtu-usUAnl5Oq84bIMrkvMuSvTYCitlhGs,6191
 sunpeek/serializable_models.py,sha256=I_GnCQZd7qDmk4n3sobRnfQdIrYl71pLg4Q-c3Bz2Z4,22210
-sunpeek-0.3.3.dist-info/COPYING.LESSER,sha256=46mU2C5kSwOnkqkw9XQAJlhBL2JAf1_uCD8lVcXyMRg,7652
-sunpeek-0.3.3.dist-info/METADATA,sha256=pvjLL8MlWmu4XiXBN7vgKQKVLO9KoDsW8Tj8CwLJH0M,15233
-sunpeek-0.3.3.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-sunpeek-0.3.3.dist-info/COPYING,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-sunpeek-0.3.3.dist-info/RECORD,,
+sunpeek-0.3.4.dist-info/COPYING.LESSER,sha256=46mU2C5kSwOnkqkw9XQAJlhBL2JAf1_uCD8lVcXyMRg,7652
+sunpeek-0.3.4.dist-info/METADATA,sha256=Wt7SfPqthdTerE8wapujikOl46zU4SB7d7VK_IiozHM,15233
+sunpeek-0.3.4.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+sunpeek-0.3.4.dist-info/COPYING,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+sunpeek-0.3.4.dist-info/RECORD,,
```

