# Comparing `tmp/qmenta_anon-1.1.dev330-py3-none-any.whl.zip` & `tmp/qmenta_anon-1.1.dev357-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9251 bytes, number of entries: 9
+Zip file size: 9272 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       65 b- defN 80-Jan-01 00:00 qmenta/__init__.py
 -rw-r--r--  2.0 unx       65 b- defN 80-Jan-01 00:00 qmenta/anon/__init__.py
 -rw-r--r--  2.0 unx     1753 b- defN 80-Jan-01 00:00 qmenta/anon/auto.py
--rw-r--r--  2.0 unx    19814 b- defN 80-Jan-01 00:00 qmenta/anon/dicom.py
+-rw-r--r--  2.0 unx    20162 b- defN 80-Jan-01 00:00 qmenta/anon/dicom.py
 -rw-r--r--  2.0 unx     1333 b- defN 80-Jan-01 00:00 qmenta/anon/nifti.py
 -rw-r--r--  2.0 unx     3731 b- defN 80-Jan-01 00:00 qmenta/anon/time_utils.py
--rw-r--r--  2.0 unx      776 b- defN 80-Jan-01 00:00 qmenta_anon-1.1.dev330.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 qmenta_anon-1.1.dev330.dist-info/WHEEL
-?rw-r--r--  2.0 unx      696 b- defN 16-Jan-01 00:00 qmenta_anon-1.1.dev330.dist-info/RECORD
-9 files, 28321 bytes uncompressed, 8059 bytes compressed:  71.5%
+-rw-r--r--  2.0 unx      677 b- defN 80-Jan-01 00:00 qmenta_anon-1.1.dev357.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 qmenta_anon-1.1.dev357.dist-info/WHEEL
+?rw-r--r--  2.0 unx      696 b- defN 16-Jan-01 00:00 qmenta_anon-1.1.dev357.dist-info/RECORD
+9 files, 28570 bytes uncompressed, 8080 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -12,17 +12,17 @@
 
 Filename: qmenta/anon/nifti.py
 Comment: 
 
 Filename: qmenta/anon/time_utils.py
 Comment: 
 
-Filename: qmenta_anon-1.1.dev330.dist-info/METADATA
+Filename: qmenta_anon-1.1.dev357.dist-info/METADATA
 Comment: 
 
-Filename: qmenta_anon-1.1.dev330.dist-info/WHEEL
+Filename: qmenta_anon-1.1.dev357.dist-info/WHEEL
 Comment: 
 
-Filename: qmenta_anon-1.1.dev330.dist-info/RECORD
+Filename: qmenta_anon-1.1.dev357.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qmenta/anon/dicom.py

```diff
@@ -221,14 +221,31 @@
     try:
         _ = header[tag].value
         return True
     except (NotImplementedError, Exception):
         return False
 
 
+def check_meta_tag(header, tag):
+    """
+    Parameters
+    ----------
+    header:
+        The DICOM header to check
+
+    tag:
+        DICOM meta tag ID to check
+    """
+    try:
+        _ = header.file_meta[tag].value
+        return True
+    except (NotImplementedError, Exception):
+        return False
+
+
 def anonymise_header_attribute(header, attribute, action):
     """
     Redact or delete the attribute from the header as specified
     by the action.
 
     Parameters
     ----------
@@ -323,19 +340,20 @@
     return {"OK": True, "error_tags": []}
 
 
 def _updateMetaInfo(header):
     """
     Set DICOM meta information if needed.
     """
-    if not check_tag(header, DicomAttribute.ImplementationClassUID.tag):
+    if not check_meta_tag(header, DicomAttribute.ImplementationClassUID.tag):
         header.file_meta.ImplementationClassUID = "1.2.3.4"
-    if not check_tag(header, DicomAttribute.MediaStorageSOPClassUID.tag):
+    if not check_meta_tag(header, DicomAttribute.MediaStorageSOPClassUID.tag):
         header.file_meta.MediaStorageSOPClassUID = "1.2.840.10008.5.1.4.1.1.2"
-    if not check_tag(header, DicomAttribute.MediaStorageSOPInstanceUID.tag):
+    if not check_meta_tag(header,
+                          DicomAttribute.MediaStorageSOPInstanceUID.tag):
         header.file_meta.MediaStorageSOPInstanceUID = "1.2.3"
 
 
 def check_anonymised_file(input_file, options={}):
     _options = {"return_lines": False, "not_found_as_error": False}
 
     _options.update(options)
```

## Comparing `qmenta_anon-1.1.dev330.dist-info/METADATA` & `qmenta_anon-1.1.dev357.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: qmenta-anon
-Version: 1.1.dev330
+Version: 1.1.dev357
 Summary: The qmenta-anon library is used to anonymize files before transferring them to the QMENTA platform.
 Author: QMENTA
 Author-email: dev@qmenta.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Dist: nibabel (>=3.2.2,<4.0.0)
 Requires-Dist: pydicom (>=2.3.0,<3.0.0)
```

## Comparing `qmenta_anon-1.1.dev330.dist-info/RECORD` & `qmenta_anon-1.1.dev357.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 qmenta/__init__.py,sha256=jv2YF__bseklT3OWEzlqJ5qE24c4aWd5F4r0TTjOrWQ,65
 qmenta/anon/__init__.py,sha256=jv2YF__bseklT3OWEzlqJ5qE24c4aWd5F4r0TTjOrWQ,65
 qmenta/anon/auto.py,sha256=08IERB8Gw4ZSHfXsqkNTJCxMnqgTR0kab-VnaZtwgxQ,1753
-qmenta/anon/dicom.py,sha256=xlw1g1FwhnWEfMR4TYyTWLFjQZbeILt7YXfO07q03K0,19814
+qmenta/anon/dicom.py,sha256=GhrlGLqXxIwsbqW4lxPtju6qt-RQCb5HfrAmSEE0mUo,20162
 qmenta/anon/nifti.py,sha256=GF17HD6-ABpL74Ys1pr0M0uLy_9al-eMB5EYaZUQwz4,1333
 qmenta/anon/time_utils.py,sha256=nxrfXsxqWPYHUB-xNwTV1Wpz9RdDKYctHqYQVUXk448,3731
-qmenta_anon-1.1.dev330.dist-info/METADATA,sha256=PhnN2Pv4Zph2Z8KdKD_TVXySGU1ZASJcgRF5KISCeL8,776
-qmenta_anon-1.1.dev330.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-qmenta_anon-1.1.dev330.dist-info/RECORD,,
+qmenta_anon-1.1.dev357.dist-info/METADATA,sha256=qn9f_X5B5qiUcCNap3BksJNGM2GVJTo9IXnYtoQQTH8,677
+qmenta_anon-1.1.dev357.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+qmenta_anon-1.1.dev357.dist-info/RECORD,,
```

