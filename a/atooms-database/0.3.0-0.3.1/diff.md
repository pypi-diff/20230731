# Comparing `tmp/atooms_database-0.3.0-py2.py3-none-any.whl.zip` & `tmp/atooms_database-0.3.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -15,13 +15,13 @@
 -rw-rw-r--  2.0 unx     6469 b- defN 23-Jun-06 11:37 atooms/database/rumd/interaction.py
 -rw-rw-r--  2.0 unx     6774 b- defN 23-Jun-06 05:58 atooms/database/storage/bernu_hiwatari_hansen_pastore/0_f61d7e58b9656cf9640f6e5754441930.xyz
 -rw-rw-r--  2.0 unx     9280 b- defN 23-Jun-06 05:58 atooms/database/storage/coslovich_pastore/0_488db481cdac35e599922a26129c3e35.xyz
 -rw-rw-r--  2.0 unx    59127 b- defN 23-Jun-06 05:58 atooms/database/storage/grigera_cavagna_giardina_parisi/0_0ac97fa8c69c320e48bd1fca80855e8a.xyz
 -rw-rw-r--  2.0 unx     4656 b- defN 23-Jun-06 05:58 atooms/database/storage/kob_andersen/0_8f4a9fe755e5c1966c10b50c9a53e6bf.xyz
 -rw-rw-r--  2.0 unx     7888 b- defN 23-Jun-06 05:58 atooms/database/storage/lennard_jones/0_13ce47602b259f7802e89e23ffd57f19.xyz
 -rw-rw-r--  2.0 unx     5927 b- defN 23-Jun-06 05:58 atooms/database/storage/lennard_jones/0_5cc3b80bc415fa5c262e83410ca65779.xyz
--rw-rw-r--  2.0 unx        0 b- defN 23-Jul-30 19:01 atooms_database-0.3.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3475 b- defN 23-Jul-30 19:01 atooms_database-0.3.0.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Jul-30 19:01 atooms_database-0.3.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       64 b- defN 23-Jul-30 19:01 atooms_database-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2441 b- defN 23-Jul-30 19:01 atooms_database-0.3.0.dist-info/RECORD
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-31 12:24 atooms_database-0.3.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3475 b- defN 23-Jul-31 12:24 atooms_database-0.3.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jul-31 12:24 atooms_database-0.3.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       64 b- defN 23-Jul-31 12:24 atooms_database-0.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2441 b- defN 23-Jul-31 12:24 atooms_database-0.3.1.dist-info/RECORD
 25 files, 151952 bytes uncompressed, 57441 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -54,23 +54,23 @@
 
 Filename: atooms/database/storage/lennard_jones/0_13ce47602b259f7802e89e23ffd57f19.xyz
 Comment: 
 
 Filename: atooms/database/storage/lennard_jones/0_5cc3b80bc415fa5c262e83410ca65779.xyz
 Comment: 
 
-Filename: atooms_database-0.3.0.dist-info/LICENSE
+Filename: atooms_database-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: atooms_database-0.3.0.dist-info/METADATA
+Filename: atooms_database-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: atooms_database-0.3.0.dist-info/WHEEL
+Filename: atooms_database-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: atooms_database-0.3.0.dist-info/top_level.txt
+Filename: atooms_database-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: atooms_database-0.3.0.dist-info/RECORD
+Filename: atooms_database-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `atooms_database-0.3.0.dist-info/METADATA` & `atooms_database-0.3.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: atooms-database
-Version: 0.3.0
+Version: 0.3.1
 Summary: Database of interaction database for classical molecular dynamics and Monte Carlo simulations
 Home-page: https://framagit.org/atooms/database
 Author: Daniele Coslovich
 Author-email: dcoslovich@units.it
 License: GPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: atooms (~=3.17)
+Requires-Dist: atooms (~=3.19)
 Requires-Dist: f2py-jit (~=0.5)
 Requires-Dist: jsonschema
 Requires-Dist: tinydb
 Requires-Dist: tqdm
 
 Atooms database
 ===============
```

## Comparing `atooms_database-0.3.0.dist-info/RECORD` & `atooms_database-0.3.1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 atooms/database/rumd/interaction.py,sha256=foD8T4xTfbYEUIhLf0qKOnGt5E_x4nknmAhoTHMAsH0,6469
 atooms/database/storage/bernu_hiwatari_hansen_pastore/0_f61d7e58b9656cf9640f6e5754441930.xyz,sha256=xak8Bt4Xakfkdoys1NijdyyN1cpMjoiqgK_ncxt3g3Q,6774
 atooms/database/storage/coslovich_pastore/0_488db481cdac35e599922a26129c3e35.xyz,sha256=QBpKZOyEb1C9hvXXQRdy74e0Sgfar8DvxaH5hKe85XE,9280
 atooms/database/storage/grigera_cavagna_giardina_parisi/0_0ac97fa8c69c320e48bd1fca80855e8a.xyz,sha256=9bZ2a_dH8F2o_HCxYgQd_-JYzaYHugiW-E1-Xd5uYmQ,59127
 atooms/database/storage/kob_andersen/0_8f4a9fe755e5c1966c10b50c9a53e6bf.xyz,sha256=KooMMAxC6GnJLHqdIgbPqyeQt9XtMEVoLVBEjDifUzg,4656
 atooms/database/storage/lennard_jones/0_13ce47602b259f7802e89e23ffd57f19.xyz,sha256=5uaL3JeCkx5xySLCg3MeCeQalnwlAtYpwq4z4ONPaCI,7888
 atooms/database/storage/lennard_jones/0_5cc3b80bc415fa5c262e83410ca65779.xyz,sha256=V3ESAodJ1_-9FR4pmvTZTJK45y-a7weZ8EBLn4dpLkE,5927
-atooms_database-0.3.0.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-atooms_database-0.3.0.dist-info/METADATA,sha256=tIjW-NyL5Tnnc1-JKkLzoLxaMSp9REsSZJnNxjlZII0,3475
-atooms_database-0.3.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-atooms_database-0.3.0.dist-info/top_level.txt,sha256=9o7UGu0YidqgwDb_N4ceklT3bPAOArDUWo-qM9G4O5A,64
-atooms_database-0.3.0.dist-info/RECORD,,
+atooms_database-0.3.1.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+atooms_database-0.3.1.dist-info/METADATA,sha256=1GLrTjc3BWV_FHSf0T1eG5wAOA5KWC0TpKXW2mbavVs,3475
+atooms_database-0.3.1.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+atooms_database-0.3.1.dist-info/top_level.txt,sha256=9o7UGu0YidqgwDb_N4ceklT3bPAOArDUWo-qM9G4O5A,64
+atooms_database-0.3.1.dist-info/RECORD,,
```

