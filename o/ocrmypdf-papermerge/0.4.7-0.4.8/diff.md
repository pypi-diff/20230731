# Comparing `tmp/ocrmypdf_papermerge-0.4.7.tar.gz` & `tmp/ocrmypdf_papermerge-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocrmypdf_papermerge-0.4.7.tar", max compression
+gzip compressed data, was "ocrmypdf_papermerge-0.4.8.tar", max compression
```

## Comparing `ocrmypdf_papermerge-0.4.7.tar` & `ocrmypdf_papermerge-0.4.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    10231 2023-07-26 12:55:18.335191 ocrmypdf_papermerge-0.4.7/LICENSE
--rw-r--r--   0        0        0      459 2023-07-26 12:55:18.335191 ocrmypdf_papermerge-0.4.7/README.md
--rw-r--r--   0        0        0      448 2023-07-26 12:55:18.335191 ocrmypdf_papermerge-0.4.7/changelog.md
--rw-r--r--   0        0        0        0 2023-07-26 12:55:18.335191 ocrmypdf_papermerge-0.4.7/ocrmypdf_papermerge/__init__.py
--rw-r--r--   0        0        0      594 2023-07-26 12:55:18.335191 ocrmypdf_papermerge-0.4.7/ocrmypdf_papermerge/generate_preview.py
--rw-r--r--   0        0        0      919 2023-07-26 12:55:18.335191 ocrmypdf_papermerge-0.4.7/ocrmypdf_papermerge/generate_svg.py
--rw-r--r--   0        0        0     1767 2023-07-26 12:55:18.335191 ocrmypdf_papermerge-0.4.7/ocrmypdf_papermerge/hocr.py
--rw-r--r--   0        0        0      664 2023-07-26 12:55:18.335191 ocrmypdf_papermerge-0.4.7/ocrmypdf_papermerge/image.py
--rw-r--r--   0        0        0     2116 2023-07-26 12:55:18.335191 ocrmypdf_papermerge-0.4.7/ocrmypdf_papermerge/plugin.py
--rw-r--r--   0        0        0      479 2023-07-26 12:55:18.335191 ocrmypdf_papermerge-0.4.7/ocrmypdf_papermerge/render.py
--rw-r--r--   0        0        0      312 2023-07-26 12:55:18.335191 ocrmypdf_papermerge-0.4.7/ocrmypdf_papermerge/templates/page.html.j2
--rw-r--r--   0        0        0      611 2023-07-26 12:55:18.335191 ocrmypdf_papermerge-0.4.7/ocrmypdf_papermerge/templates/page.svg.j2
--rw-r--r--   0        0        0     2544 2023-07-26 12:55:18.335191 ocrmypdf_papermerge-0.4.7/ocrmypdf_papermerge/utils.py
--rw-r--r--   0        0        0     1376 2023-07-26 12:55:18.335191 ocrmypdf_papermerge-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     1609 1970-01-01 00:00:00.000000 ocrmypdf_papermerge-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0    10231 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/LICENSE
+-rw-r--r--   0        0        0      459 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/README.md
+-rw-r--r--   0        0        0      448 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/changelog.md
+-rw-r--r--   0        0        0        0 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/__init__.py
+-rw-r--r--   0        0        0      594 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/generate_preview.py
+-rw-r--r--   0        0        0      919 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/generate_svg.py
+-rw-r--r--   0        0        0     1767 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/hocr.py
+-rw-r--r--   0        0        0      664 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/image.py
+-rw-r--r--   0        0        0     2116 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/plugin.py
+-rw-r--r--   0        0        0      479 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/render.py
+-rw-r--r--   0        0        0      312 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/templates/page.html.j2
+-rw-r--r--   0        0        0      611 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/templates/page.svg.j2
+-rw-r--r--   0        0        0     2544 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/utils.py
+-rw-r--r--   0        0        0     1375 2023-07-31 06:09:43.110589 ocrmypdf_papermerge-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 ocrmypdf_papermerge-0.4.8/PKG-INFO
```

### Comparing `ocrmypdf_papermerge-0.4.7/LICENSE` & `ocrmypdf_papermerge-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ocrmypdf_papermerge-0.4.7/ocrmypdf_papermerge/generate_preview.py` & `ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/generate_preview.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf_papermerge-0.4.7/ocrmypdf_papermerge/generate_svg.py` & `ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/generate_svg.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf_papermerge-0.4.7/ocrmypdf_papermerge/hocr.py` & `ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/hocr.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf_papermerge-0.4.7/ocrmypdf_papermerge/image.py` & `ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/image.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf_papermerge-0.4.7/ocrmypdf_papermerge/plugin.py` & `ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/plugin.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf_papermerge-0.4.7/ocrmypdf_papermerge/templates/page.svg.j2` & `ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/templates/page.svg.j2`

 * *Files identical despite different names*

### Comparing `ocrmypdf_papermerge-0.4.7/ocrmypdf_papermerge/utils.py` & `ocrmypdf_papermerge-0.4.8/ocrmypdf_papermerge/utils.py`

 * *Files identical despite different names*

### Comparing `ocrmypdf_papermerge-0.4.7/pyproject.toml` & `ocrmypdf_papermerge-0.4.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ocrmypdf-papermerge"
-version = "0.4.7"
+version = "0.4.8"
 description = "OCRmyPDF plugin to generate SVG files for Papermerge"
 authors = ["Eugen Ciur <eugen@papermerge.com>"]
 maintainers = ["Eugen Ciur <eugen@papermerge.com>"]
 license = "Apache-2.0"
 include = ["LICENSE", "changelog.md", "README.md", "ocrmypdf_papermerge/templates/*"]
 readme = "README.md"
 classifiers = [
@@ -20,15 +20,15 @@
 ]
 homepage = "https://github.com/papermerge/OCRmyPDF_papermerge"
 repository = "https://github.com/papermerge/OCRmyPDF_papermerge"
 keywords = ["OCR", "PDF", "OCRmyPDF", "Document Management System"]
 
 
 [tool.poetry.dependencies]
-python = ">=3.8, <3.12"
+python = ">=3.8, <4.0"
 ocrmypdf = "^14.3.0"
 Jinja2 = "^3.1.2"
 lxml = "^4.9.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pycodestyle = "^2.8.0"
```

### Comparing `ocrmypdf_papermerge-0.4.7/PKG-INFO` & `ocrmypdf_papermerge-0.4.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ocrmypdf-papermerge
-Version: 0.4.7
+Version: 0.4.8
 Summary: OCRmyPDF plugin to generate SVG files for Papermerge
 Home-page: https://github.com/papermerge/OCRmyPDF_papermerge
 License: Apache-2.0
 Keywords: OCR,PDF,OCRmyPDF,Document Management System
 Author: Eugen Ciur
 Author-email: eugen@papermerge.com
 Maintainer: Eugen Ciur
 Maintainer-email: eugen@papermerge.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

