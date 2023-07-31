# Comparing `tmp/fileformats-0.8.1.tar.gz` & `tmp/fileformats-0.8.2.tar.gz`

## Comparing `fileformats-0.8.1.tar` & `fileformats-0.8.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/archive/__init__.py
--rw-r--r--   0        0        0    18026 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/audio/__init__.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/_version.py
--rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/converter.py
--rw-r--r--   0        0        0     9785 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/datatype.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/exceptions.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/field.py
--rw-r--r--   0        0        0    46110 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/fileset.py
--rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/mark.py
--rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/mixin.py
--rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/utils.py
--rw-r--r--   0        0        0     9029 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/tests/test_classifiers.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/tests/test_converter.py
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/tests/test_detection.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/tests/test_general.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/tests/test_mime.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/tests/test_mixin.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/tests/test_subpackages.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/tests/test_test_extras.py
--rw-r--r--   0        0        0    11504 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/core/tests/test_utils.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/document/__init__.py
--rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/field/__init__.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/field/tests/test_fields.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/field/tests/test_fields_mime.py
--rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/generic/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/image/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/image/base.py
--rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/image/notclassifiedyet.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/image/raster.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/image/vector.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/image/tests/test_image_raster.py
--rw-r--r--   0        0        0     8838 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/misc/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/misc/medical.py
--rw-r--r--   0        0        0    83996 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/misc/unclassified.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/model/__init__.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/serialization/__init__.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/testing/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/testing/basic.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/testing/classifiers.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/testing/headers.py
--rw-r--r--   0        0        0     8438 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/text/__init__.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 fileformats-0.8.1/fileformats/video/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.8.1/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.8.1/AUTHORS
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.8.1/LICENSE
--rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 fileformats-0.8.1/README.rst
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 fileformats-0.8.1/pyproject.toml
--rw-r--r--   0        0        0    23194 2020-02-02 00:00:00.000000 fileformats-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/archive/__init__.py
+-rw-r--r--   0        0        0    18026 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/audio/__init__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/_version.py
+-rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/converter.py
+-rw-r--r--   0        0        0     9785 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/datatype.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/exceptions.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/field.py
+-rw-r--r--   0        0        0    46180 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/fileset.py
+-rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/mark.py
+-rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/mixin.py
+-rw-r--r--   0        0        0    10283 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/utils.py
+-rw-r--r--   0        0        0     9029 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/tests/test_classifiers.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/tests/test_converter.py
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/tests/test_detection.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/tests/test_general.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/tests/test_mime.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/tests/test_mixin.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/tests/test_subpackages.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/tests/test_test_extras.py
+-rw-r--r--   0        0        0    12335 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/core/tests/test_utils.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/document/__init__.py
+-rw-r--r--   0        0        0     5558 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/field/__init__.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/field/tests/test_fields.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/field/tests/test_fields_mime.py
+-rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/generic/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/image/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/image/base.py
+-rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/image/notclassifiedyet.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/image/raster.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/image/vector.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/image/tests/test_image_raster.py
+-rw-r--r--   0        0        0     8838 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/misc/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/misc/medical.py
+-rw-r--r--   0        0        0    83996 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/misc/unclassified.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/model/__init__.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/serialization/__init__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/testing/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/testing/basic.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/testing/classifiers.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/testing/headers.py
+-rw-r--r--   0        0        0     8443 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/text/__init__.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 fileformats-0.8.2/fileformats/video/__init__.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.8.2/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.8.2/AUTHORS
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.8.2/LICENSE
+-rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 fileformats-0.8.2/README.rst
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 fileformats-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0    23194 2020-02-02 00:00:00.000000 fileformats-0.8.2/PKG-INFO
```

### Comparing `fileformats-0.8.1/fileformats/archive/__init__.py` & `fileformats-0.8.2/fileformats/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/audio/__init__.py` & `fileformats-0.8.2/fileformats/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/core/converter.py` & `fileformats-0.8.2/fileformats/core/converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/core/datatype.py` & `fileformats-0.8.2/fileformats/core/datatype.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/core/exceptions.py` & `fileformats-0.8.2/fileformats/core/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,18 +10,14 @@
     "No converters exist between formats"
 
 
 class FormatRecognitionError(KeyError, FileFormatsError):
     "Did not find a format class corresponding to a MIME, or MIME-like, type string"
 
 
-class MissingExtendedDepenciesError(FileFormatsError):
-    "'extended' install extra wasn't installed required for advanced behaviour"
-
-
 class FileFormatsExtrasError(FileFormatsError):
     """If there is an "extras hook" in the datatype class but no methods have been
     registered on it"""
 
 
 class FileFormatsExtrasPkgUninstalledError(FileFormatsExtrasError):
     """If there is an "extras hook" in the datatype class and a extras package on PyPI
```

### Comparing `fileformats-0.8.1/fileformats/core/field.py` & `fileformats-0.8.2/fileformats/core/field.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/core/fileset.py` & `fileformats-0.8.2/fileformats/core/fileset.py`

 * *Files 0% similar despite different names*

```diff
@@ -917,14 +917,16 @@
             )
         return decomposed_fspaths
 
     @classmethod
     def decompose_fspath(
         cls, fspath: Path, mode: ExtensionDecomposition = ExtensionDecomposition.single
     ) -> ty.Tuple[Path, str, str]:
+        if isinstance(fspath, str):
+            fspath = Path(fspath)
         """Decompose an arbitrary file-system path into parent dir, stem and extension
         given the assumption on what constitutes an extension"""
         if mode == cls.ExtensionDecomposition.multiple:
             ext = "".join(fspath.suffixes)
             stem = fspath.name[: -len(ext)]
         elif mode == cls.ExtensionDecomposition.single:
             stem = fspath.stem
```

### Comparing `fileformats-0.8.1/fileformats/core/mark.py` & `fileformats-0.8.2/fileformats/core/mark.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/core/mixin.py` & `fileformats-0.8.2/fileformats/core/mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/core/utils.py` & `fileformats-0.8.2/fileformats/core/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import urllib.request
 import urllib.error
 import os
 import logging
 import pkgutil
 from contextlib import contextmanager
 from fileformats.core.exceptions import (
-    MissingExtendedDepenciesError,
     FileFormatsError,
 )
 import fileformats.core
 
 logger = logging.getLogger("fileformats")
 
 
@@ -75,17 +74,74 @@
             and (include_generic or namespace != "generic")
         ):
             matches.append(frmt)
     return matches
 
 
 def from_mime(mime_str: str):
+    """Resolves a MIME type (or MIME-like) string into the corresponding type
+
+    Parameters
+    ----------
+    mime_str : str
+        the MIME type, or MIME-like (i.e. using the fileformats namespace scheme
+        instead of putting all non-standard types into application/*), string to
+        resolve
+
+    Returns
+    -------
+    datatype : type
+        the resolved datatype
+    """
+    if mime_str.endswith(LIST_MIME):
+        item_mime = mime_str[: -len(LIST_MIME)]
+        if item_mime.startswith("[") and item_mime.endswith("]"):
+            item_mime = item_mime[1:-1]
+        return ty.List[from_mime(item_mime)]
+    if "," in mime_str:
+        return ty.Union.__getitem__(tuple(from_mime(t) for t in mime_str.split(",")))
     return fileformats.core.DataType.from_mime(mime_str)
 
 
+def to_mime(datatype: type, official=False):
+    """Returns the mime-type or mime-like (i.e. using fileformats namespaces instead
+    of putting all non-standard types in the applications/* registry) string corresponding
+    to the given datatype
+
+    Parameters
+    ----------
+    datatype : type
+        the datatype to get the mime string for
+    official : bool
+        whether to use the official mime-type instead of mime-like
+
+    Returns
+    -------
+    mime_str : str
+        the MIME type string if `iana=True`, or MIME-like (i.e. using the fileformats
+        namespace scheme instead of putting all non-standard types into application/*)
+        if not
+    """
+    origin = ty.get_origin(datatype)
+    if official and (origin or datatype.namespace == "field"):
+        raise TypeError(
+            f"Cannot convert {datatype} to official mime-type as it is not a proper "
+            'file-type, please use official=False to convert to "mime-like" string instead'
+        )
+    if origin is list:
+        item_mime = to_mime(ty.get_args(datatype)[0])
+        if "," in item_mime:
+            item_mime = "[" + item_mime + "]"
+        item_mime += LIST_MIME
+        return item_mime
+    if origin is ty.Union:
+        return ",".join(t.mime_like for t in ty.get_args(datatype))
+    return datatype.mime_type if official else datatype.mime_like
+
+
 def subpackages(exclude: ty.Sequence[str] = _excluded_subpackages):
     """Iterates over all subpackages within the fileformats namespace
 
     Parameters
     ----------
     exclude : ty.Sequence[str], optional
         whether to include the testing subpackage, by default ["core", "testing"]
@@ -144,45 +200,14 @@
     def __init__(self, f):
         self.f = f
 
     def __get__(self, obj, owner):
         return self.f(owner)
 
 
-class MissingExtendedDependency:
-    """Used as a placeholder for package dependencies that are only installed with the
-    "extended" install extra.
-
-    Parameters
-    ----------
-    pkg_name : str
-        name of the package to act as a placeholder for
-    module_path : str
-        path of the module, i.e. the value of the '__name__' global variable
-    """
-
-    def __init__(self, pkg_name: str, module_path: str):
-        self.pkg_name = pkg_name
-        module_parts = module_path.split(".")
-        assert module_parts[0] == "fileformats"
-        if module_parts[1] in STANDARD_NAMESPACES:
-            self.required_in = "fileformats"
-        else:
-            self.required_in = f"fileformats-{module_parts[1]}"
-
-    def __getattr__(self, _):
-        raise MissingExtendedDepenciesError(
-            f"Not able to access extended behaviour in {self.required_in} as required "
-            f"package '{self.pkg_name}' was not installed. Please reinstall "
-            f"{self.required_in} with 'extended' install extra to access extended "
-            f"behaviour of the format classes (such as loading and conversion), i.e.\n\n"
-            f"    $ python3 -m pip install {self.required_in}[extended]"
-        )
-
-
 STANDARD_NAMESPACES = [
     "archive",
     "audio",
     "document",
     "image",
     "misc",
     "model",
@@ -321,7 +346,10 @@
     try:
         importlib.import_module(extras_pkg)
     except ImportError:
         extras_imported = False
     else:
         extras_imported = True
     return extras_imported, extras_pkg, extras_pypi
+
+
+LIST_MIME = "+list-of"
```

### Comparing `fileformats-0.8.1/fileformats/core/tests/test_classifiers.py` & `fileformats-0.8.2/fileformats/core/tests/test_classifiers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/core/tests/test_converter.py` & `fileformats-0.8.2/fileformats/core/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/core/tests/test_detection.py` & `fileformats-0.8.2/fileformats/core/tests/test_detection.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/core/tests/test_general.py` & `fileformats-0.8.2/fileformats/core/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/core/tests/test_mime.py` & `fileformats-0.8.2/fileformats/core/tests/test_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/core/tests/test_mixin.py` & `fileformats-0.8.2/fileformats/core/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/core/tests/test_subpackages.py` & `fileformats-0.8.2/fileformats/core/tests/test_subpackages.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/core/tests/test_test_extras.py` & `fileformats-0.8.2/fileformats/core/tests/test_test_extras.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/core/tests/test_utils.py` & `fileformats-0.8.2/fileformats/core/tests/test_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,66 @@
 from pathlib import Path
 import os.path
 import random
 import shutil
+import typing as ty
 import time
 import pytest
 from fileformats.core import FileSet, mark
 from fileformats.generic import File, Directory, FsObject
 from fileformats.core.mixin import WithSeparateHeader
 from fileformats.core.utils import (
     find_matching,
-    MissingExtendedDependency,
+    to_mime,
+    from_mime,
 )
-from fileformats.core.exceptions import MissingExtendedDepenciesError, FileFormatsError
+from fileformats.core.exceptions import FileFormatsError
+from fileformats.testing import Foo, Bar
 import fileformats.text
 from conftest import write_test_file
 
 
-class Bar(File):
-    ext = ".bar"
+class Mario(File):
+    ext = ".mario"
 
 
-class Foo(WithSeparateHeader, File):
-    ext = ".foo"
-    header_type = Bar
+class Luigi(WithSeparateHeader, File):
+    ext = ".luigi"
+    header_type = Mario
 
 
-class Baz(Directory):
-    content_types = (Bar,)
+class Bowser(Directory):
+    content_types = (Mario,)
 
 
 @pytest.fixture
-def baz_dir(work_dir):
-    baz_dir = work_dir / "baz"
-    baz_dir.mkdir()
+def bowser_dir(work_dir):
+    bowser_dir = work_dir / "bowser"
+    bowser_dir.mkdir()
     for i in range(5):
-        bar_fspath = baz_dir / f"{i}.bar"
+        bar_fspath = bowser_dir / f"{i}.mario"
         write_test_file(bar_fspath)
-    return Baz(baz_dir)
+    return Bowser(bowser_dir)
 
 
 @pytest.fixture
-def foo_file(work_dir):
-    foo_fspath = work_dir / "x.foo"
-    write_test_file(foo_fspath)
-    bar_fspath = work_dir / "y.bar"
+def luigi_file(work_dir):
+    luigi_fspath = work_dir / "x.luigi"
+    write_test_file(luigi_fspath)
+    bar_fspath = work_dir / "y.mario"
     write_test_file(bar_fspath)
-    return Foo([foo_fspath, bar_fspath])
+    return Luigi([luigi_fspath, bar_fspath])
 
 
-@pytest.fixture(params=["foo", "baz"])
-def fsobject(foo_file, baz_dir, request):
-    if request.param == "foo":
-        return foo_file
-    elif request.param == "baz":
-        return baz_dir
+@pytest.fixture(params=["luigi", "bowser"])
+def fsobject(luigi_file, bowser_dir, request):
+    if request.param == "luigi":
+        return luigi_file
+    elif request.param == "bowser":
+        return bowser_dir
     else:
         assert False
 
 
 @pytest.fixture
 def dest_dir(work_dir):
     dest_dir = work_dir / "new-dir"
@@ -192,19 +195,19 @@
     fileset = FileSet(fspaths)
 
     cpy = fileset.copy(dest_dir=dest_dir, collation="adjacent", new_stem="newfile")
     assert all(p.parent == dest_dir for p in cpy.fspaths)
     assert all(p.stem == "newfile" for p in cpy.fspaths)
 
 
-def test_copy_collation_with_stem_not_adjacent(foo_file: Foo, dest_dir):
+def test_copy_collation_with_stem_not_adjacent(luigi_file: Luigi, dest_dir):
     with pytest.raises(
         FileFormatsError, match="when collation is not set to 'adjacent'"
     ):
-        foo_file.copy(dest_dir, collation="any", new_stem="new")
+        luigi_file.copy(dest_dir, collation="any", new_stem="new")
 
 
 def test_copy_collation_leave_diff_dir(work_dir: Path, dest_dir: Path):
     a = work_dir / "a" / "file.x"
     b = work_dir / "b" / "file.y"
     c = work_dir / "c" / "file.z"
     fspaths = (a, b, c)
@@ -227,85 +230,81 @@
     ):
         fileset.copy(dest_dir=dest_dir, mode="leave", collation="adjacent")
 
 
 def test_copy_ext(work_dir):
     assert (
         File.copy_ext(
-            work_dir / "x.foo.bar",
+            work_dir / "x.luigi.mario",
             work_dir / "y",
             decomposition_mode=FileSet.ExtensionDecomposition.none,
         )
         == work_dir / "y"
     )
     assert (
         File.copy_ext(
-            work_dir / "x.foo.bar",
+            work_dir / "x.luigi.mario",
             work_dir / "y",
             decomposition_mode=FileSet.ExtensionDecomposition.single,
         )
-        == work_dir / "y.bar"
+        == work_dir / "y.mario"
     )
     assert (
         File.copy_ext(
-            work_dir / "x.foo.bar",
+            work_dir / "x.luigi.mario",
             work_dir / "y",
             decomposition_mode=FileSet.ExtensionDecomposition.multiple,
         )
-        == work_dir / "y.foo.bar"
+        == work_dir / "y.luigi.mario"
+    )
+    assert (
+        Mario.copy_ext(work_dir / "x.luigi.mario", work_dir / "y")
+        == work_dir / "y.mario"
     )
-    assert Bar.copy_ext(work_dir / "x.foo.bar", work_dir / "y") == work_dir / "y.bar"
 
 
 def test_decompose_fspaths(work_dir):
-    class FooBar(File):
-        ext = ".foo.bar"
+    class LuigiMario(File):
+        ext = ".luigi.mario"
 
-    class DoubleBar(FileSet):
+    class DoubleMario(FileSet):
         @mark.required
         @property
         def bar(self):
-            return Bar(self.select_by_ext(Bar))
+            return Mario(self.select_by_ext(Mario))
 
         @mark.required
         @property
-        def foo_bar(self):
-            return FooBar(self.select_by_ext(FooBar))
+        def luigi_bar(self):
+            return LuigiMario(self.select_by_ext(LuigiMario))
 
-    fspath = work_dir / "file.foo.bar"
+    fspath = work_dir / "file.luigi.mario"
     Path.touch(fspath)
-    double_bar = DoubleBar(fspath)
+    double_bar = DoubleMario(fspath)
 
     with pytest.warns(match="whereas it is also interpreted as a"):
         decomposed = double_bar.decomposed_fspaths()
 
-    assert decomposed == [(work_dir, "file.foo", ".bar")]
+    assert decomposed == [(work_dir, "file.luigi", ".mario")]
 
 
 def test_format_detection(work_dir):
     text_file = work_dir / "text.txt"
 
     with open(text_file, "w") as f:
         f.write("sample text")
 
     detected = find_matching(text_file, standard_only=True)
     assert sorted(detected, key=lambda f: f.mime_like) == [
         fileformats.text.Prs_Fallenstein_Rst,
         fileformats.text.Prs_Prop_Logic,
-        fileformats.text.Txt,
+        fileformats.text.TextFile,
     ]
 
 
-def test_missing_dependency():
-    missing_dep = MissingExtendedDependency("missing_dep", "fileformats.image")
-
-    with pytest.raises(MissingExtendedDepenciesError):
-        missing_dep.an_attr
-
-
 def test_hash(tmp_path: Path):
     file_1 = tmp_path / "file_1.txt"
     file_2 = tmp_path / "file_2.txt"
     file_1.write_text("hello")
     file_2.write_text("hello")
 
     assert File(file_1).hash() == File(file_2).hash()
@@ -317,15 +316,15 @@
     file_1.write_text("hello")
     file_2.write_text("hi")
 
     assert File(file_1).hash() != File(file_2).hash()
 
 
 def test_hash_dir(tmp_path: Path):
-    dir1 = tmp_path / "foo"
+    dir1 = tmp_path / "luigi"
     dir2 = tmp_path / "bar"
     for d in (dir1, dir2):
         d.mkdir()
         for i in range(3):
             f = d / f"{i}.txt"
             f.write_text(str(i))
 
@@ -384,7 +383,36 @@
 def test_hash_files(fsobject: FsObject, work_dir: Path, dest_dir: Path):
     file_hashes = fsobject.hash_files(relative_to=work_dir)
     assert sorted(Path(p) for p in file_hashes) == sorted(
         p.relative_to(work_dir) for p in fsobject.all_file_paths
     )
     cpy = fsobject.copy(dest_dir)
     assert cpy.hash_files() == fsobject.hash_files()
+
+
+def test_to_from_mime_roundtrip():
+    mime_str = to_mime(Foo)
+    assert isinstance(mime_str, str)
+    assert from_mime(mime_str) == Foo
+
+
+def test_to_from_list_mime_roundtrip():
+    mime_str = to_mime(ty.List[Foo])
+    assert isinstance(mime_str, str)
+    assert from_mime(mime_str) == ty.List[Foo]
+
+
+def test_to_from_union_mime_roundtrip():
+    mime_str = to_mime(ty.Union[Foo, Bar])
+    assert isinstance(mime_str, str)
+    assert from_mime(mime_str) == ty.Union[Foo, Bar]
+
+
+def test_to_from_list_union_mime_roundtrip():
+    mime_str = to_mime(ty.List[ty.Union[Foo, Bar]])
+    assert isinstance(mime_str, str)
+    assert from_mime(mime_str) == ty.List[ty.Union[Foo, Bar]]
+
+
+def test_official_mime_fail():
+    with pytest.raises(TypeError, match="as it is not a proper file-type"):
+        to_mime(ty.List[Foo], official=True)
```

### Comparing `fileformats-0.8.1/fileformats/document/__init__.py` & `fileformats-0.8.2/fileformats/document/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/field/__init__.py` & `fileformats-0.8.2/fileformats/field/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/field/tests/test_fields.py` & `fileformats-0.8.2/fileformats/field/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/field/tests/test_fields_mime.py` & `fileformats-0.8.2/fileformats/field/tests/test_fields_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/generic/__init__.py` & `fileformats-0.8.2/fileformats/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/image/__init__.py` & `fileformats-0.8.2/fileformats/image/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/image/notclassifiedyet.py` & `fileformats-0.8.2/fileformats/image/notclassifiedyet.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/image/raster.py` & `fileformats-0.8.2/fileformats/image/raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/image/tests/test_image_raster.py` & `fileformats-0.8.2/fileformats/image/tests/test_image_raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/misc/__init__.py` & `fileformats-0.8.2/fileformats/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/misc/unclassified.py` & `fileformats-0.8.2/fileformats/misc/unclassified.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/model/__init__.py` & `fileformats-0.8.2/fileformats/model/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/serialization/__init__.py` & `fileformats-0.8.2/fileformats/serialization/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from pathlib import Path
 import json
 from ..core import __version__, mark, DataType
 from ..core.mixin import WithClassifiers
 from ..generic import File
 from ..core.exceptions import FormatMismatchError
-from ..core.utils import MissingExtendedDependency
 
 
 class Schema(DataType):
     """Base class for all serialization schemas (can be used for abstract schemas that
     don't actually have a formal definition)"""
 
     pass
```

### Comparing `fileformats-0.8.1/fileformats/testing/classifiers.py` & `fileformats-0.8.2/fileformats/testing/classifiers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/testing/headers.py` & `fileformats-0.8.2/fileformats/testing/headers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/fileformats/text/__init__.py` & `fileformats-0.8.2/fileformats/text/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 # General formats
 class Plain(Text):
     iana_mime = "text/plain"
 
 
-class Txt(Text):
+class TextFile(Text):
     ext = ".txt"
 
 
 class Csv(Text):
     ext = ".csv"
     iana_mime = "text/csv"
```

### Comparing `fileformats-0.8.1/fileformats/video/__init__.py` & `fileformats-0.8.2/fileformats/video/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/LICENSE` & `fileformats-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/README.rst` & `fileformats-0.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/pyproject.toml` & `fileformats-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fileformats-0.8.1/PKG-INFO` & `fileformats-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats
-Version: 0.8.1
+Version: 0.8.2
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```

