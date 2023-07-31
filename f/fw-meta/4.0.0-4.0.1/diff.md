# Comparing `tmp/fw_meta-4.0.0-py3-none-any.whl.zip` & `tmp/fw_meta-4.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 15483 bytes, number of entries: 9
+Zip file size: 15478 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      386 b- defN 80-Jan-01 00:00 fw_meta/__init__.py
 -rw-r--r--  2.0 unx      665 b- defN 80-Jan-01 00:00 fw_meta/aliases.py
 -rw-r--r--  2.0 unx     7720 b- defN 80-Jan-01 00:00 fw_meta/exports.py
 -rw-r--r--  2.0 unx    25025 b- defN 80-Jan-01 00:00 fw_meta/imports.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fw_meta/py.typed
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_meta-4.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     9983 b- defN 80-Jan-01 00:00 fw_meta-4.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_meta-4.0.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      664 b- defN 16-Jan-01 00:00 fw_meta-4.0.0.dist-info/RECORD
-9 files, 45609 bytes uncompressed, 14355 bytes compressed:  68.5%
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_meta-4.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9976 b- defN 80-Jan-01 00:00 fw_meta-4.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_meta-4.0.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx      664 b- defN 16-Jan-01 00:00 fw_meta-4.0.1.dist-info/RECORD
+9 files, 45602 bytes uncompressed, 14350 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: fw_meta/imports.py
 Comment: 
 
 Filename: fw_meta/py.typed
 Comment: 
 
-Filename: fw_meta-4.0.0.dist-info/LICENSE
+Filename: fw_meta-4.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: fw_meta-4.0.0.dist-info/METADATA
+Filename: fw_meta-4.0.1.dist-info/METADATA
 Comment: 
 
-Filename: fw_meta-4.0.0.dist-info/WHEEL
+Filename: fw_meta-4.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: fw_meta-4.0.0.dist-info/RECORD
+Filename: fw_meta-4.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fw_meta-4.0.0.dist-info/LICENSE` & `fw_meta-4.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_meta-4.0.0.dist-info/METADATA` & `fw_meta-4.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fw-meta
-Version: 4.0.0
+Version: 4.0.1
 Summary: Flywheel metadata extraction.
 Home-page: https://gitlab.com/flywheel-io/tools/lib/fw-meta
 License: MIT
 Keywords: Flywheel,DICOM,metadata,extract
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.8,<4.0
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: fw-utils (>=4.2.5,<5.0.0)
+Requires-Dist: fw-utils (>=4.2.5)
 Requires-Dist: pydantic (>=1.7.3,<2.0.0)
 Project-URL: Documentation, https://gitlab.com/flywheel-io/tools/lib/fw-meta
 Project-URL: Repository, https://gitlab.com/flywheel-io/tools/lib/fw-meta
 Description-Content-Type: text/markdown
 
 # fw-meta
```

## Comparing `fw_meta-4.0.0.dist-info/RECORD` & `fw_meta-4.0.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 fw_meta/__init__.py,sha256=WrDqzdSjEJ5mc0JE3p4Cqbkhi8LI33lWdzB5PBsII18,386
 fw_meta/aliases.py,sha256=2XTtEHVDUVbG31fYxM9XBsOrTZEhI-_nSB7SVJisme8,665
 fw_meta/exports.py,sha256=ArQ74jXynRc6w8BwI8jwZd7m_34QYgfVdfI2rrcsuuQ,7720
 fw_meta/imports.py,sha256=CqEpEM6_yDfqYrDbZ1SvtKhH0jHH7i0n4_azDi1D71I,25025
 fw_meta/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-fw_meta-4.0.0.dist-info/LICENSE,sha256=3QLwoJgDkLWRKwcyYzPn3vLqTHhbdltfjFYeBOZSlDY,1078
-fw_meta-4.0.0.dist-info/METADATA,sha256=pzzD06V0nVsNtw_xXIUUw9a9fvJ4QrmK-abJpCc9xIY,9983
-fw_meta-4.0.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-fw_meta-4.0.0.dist-info/RECORD,,
+fw_meta-4.0.1.dist-info/LICENSE,sha256=3QLwoJgDkLWRKwcyYzPn3vLqTHhbdltfjFYeBOZSlDY,1078
+fw_meta-4.0.1.dist-info/METADATA,sha256=wejRt3oYXaxQKR1mdlZdd7S4nX-AndVkLZB7d4gPn7w,9976
+fw_meta-4.0.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+fw_meta-4.0.1.dist-info/RECORD,,
```

