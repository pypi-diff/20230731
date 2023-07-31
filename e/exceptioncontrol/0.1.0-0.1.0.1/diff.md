# Comparing `tmp/exceptioncontrol-0.1.0.tar.gz` & `tmp/exceptioncontrol-0.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exceptioncontrol-0.1.0.tar", max compression
+gzip compressed data, was "exceptioncontrol-0.1.0.1.tar", max compression
```

## Comparing `exceptioncontrol-0.1.0.tar` & `exceptioncontrol-0.1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      657 2023-06-12 02:59:49.659262 exceptioncontrol-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1732 2023-05-31 03:25:27.620372 exceptioncontrol-0.1.0/LICENSE
--rw-r--r--   0        0        0     1815 2023-06-12 03:16:13.248906 exceptioncontrol-0.1.0/README.md
--rw-r--r--   0        0        0     1597 2023-06-12 03:21:35.118772 exceptioncontrol-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    14612 2023-06-12 02:59:49.659262 exceptioncontrol-0.1.0/src/exceptioncontrol/ExceptionControl.py
--rw-r--r--   0        0        0     2445 2023-06-12 02:59:49.659262 exceptioncontrol-0.1.0/src/exceptioncontrol/__init__.py
--rw-r--r--   0        0        0     2441 2023-06-12 02:59:49.659262 exceptioncontrol-0.1.0/src/exceptioncontrol/unittests/__init__.py
--rw-r--r--   0        0        0     3423 2023-06-12 02:59:49.659262 exceptioncontrol-0.1.0/src/exceptioncontrol/unittests/common.py
--rw-r--r--   0        0        0    37630 2023-06-12 02:59:49.659262 exceptioncontrol-0.1.0/src/exceptioncontrol/unittests/test_ExceptionControl.py
--rw-r--r--   0        0        0     2460 2023-06-12 02:59:49.659262 exceptioncontrol-0.1.0/src/exceptioncontrol/version.py
--rw-r--r--   0        0        0     3238 1970-01-01 00:00:00.000000 exceptioncontrol-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      761 2023-07-31 00:14:19.931617 exceptioncontrol-0.1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1732 2023-05-31 03:25:27.620372 exceptioncontrol-0.1.0.1/LICENSE
+-rw-r--r--   0        0        0     1815 2023-06-12 03:16:13.248906 exceptioncontrol-0.1.0.1/README.md
+-rw-r--r--   0        0        0     1603 2023-07-31 00:15:54.351601 exceptioncontrol-0.1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    14612 2023-06-12 02:59:49.659262 exceptioncontrol-0.1.0.1/src/exceptioncontrol/ExceptionControl.py
+-rw-r--r--   0        0        0     2445 2023-06-12 02:59:49.659262 exceptioncontrol-0.1.0.1/src/exceptioncontrol/__init__.py
+-rw-r--r--   0        0        0     2441 2023-06-12 02:59:49.659262 exceptioncontrol-0.1.0.1/src/exceptioncontrol/unittests/__init__.py
+-rw-r--r--   0        0        0     3423 2023-06-12 02:59:49.659262 exceptioncontrol-0.1.0.1/src/exceptioncontrol/unittests/common.py
+-rw-r--r--   0        0        0    37630 2023-06-12 02:59:49.659262 exceptioncontrol-0.1.0.1/src/exceptioncontrol/unittests/test_ExceptionControl.py
+-rw-r--r--   0        0        0     2462 2023-07-31 00:14:19.931617 exceptioncontrol-0.1.0.1/src/exceptioncontrol/version.py
+-rw-r--r--   0        0        0     3244 1970-01-01 00:00:00.000000 exceptioncontrol-0.1.0.1/PKG-INFO
```

### Comparing `exceptioncontrol-0.1.0/CHANGELOG.md` & `exceptioncontrol-0.1.0.1/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -18,16 +18,21 @@
 ### Changed
 ### Deprecated
 ### Removed
 ### Fixed
 ### Internal
 ### Security
 ### TODO
+### Documentation
 -->
 
+## [0.1.0.1] - 2023-07-31
+### Documentation
+- Added some minor documentation updates
+
 
 ## [0.1.0] - 2023-06-01
 ### Added
 ### Changed
 - Initial extraction from ConfigParserEnhanced
 - Develop individualized packaging for ExceptionControl
 ### Internal
```

### Comparing `exceptioncontrol-0.1.0/LICENSE` & `exceptioncontrol-0.1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exceptioncontrol-0.1.0/README.md` & `exceptioncontrol-0.1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `exceptioncontrol-0.1.0/pyproject.toml` & `exceptioncontrol-0.1.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "exceptioncontrol"
 description = "Helper class for exception handling"
-version = "0.1.0"
+version = "0.1.0.1"
 license = "LICENSE"
 readme = "README.md"
 keywords = [
     "Exception Handling",
     "Debugging"
 ]
 repository = "https://gitlab.com/semantik-software/code/python/ExceptionControl"
 documentation = "https://semantik-software.gitlab.io/code/python/ExceptionControl"
 authors = [
-    "William McLendon <wcmclen@hotmail.com>",
+    "William <Semantik-Codeworks@outlook.com>",
 ]
 maintainers = [
-    "William McLendon <wcmclen@hotmail.com>",
+    "William <Semantik-Codeworks@outlook.com>",
 ]
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Intended Audience :: System Administrators',
     'Intended Audience :: Other Audience',
     'Programming Language :: Python :: 3.6',
```

### Comparing `exceptioncontrol-0.1.0/src/exceptioncontrol/ExceptionControl.py` & `exceptioncontrol-0.1.0.1/src/exceptioncontrol/ExceptionControl.py`

 * *Files identical despite different names*

### Comparing `exceptioncontrol-0.1.0/src/exceptioncontrol/__init__.py` & `exceptioncontrol-0.1.0.1/src/exceptioncontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `exceptioncontrol-0.1.0/src/exceptioncontrol/unittests/__init__.py` & `exceptioncontrol-0.1.0.1/src/exceptioncontrol/unittests/__init__.py`

 * *Files identical despite different names*

### Comparing `exceptioncontrol-0.1.0/src/exceptioncontrol/unittests/common.py` & `exceptioncontrol-0.1.0.1/src/exceptioncontrol/unittests/common.py`

 * *Files identical despite different names*

### Comparing `exceptioncontrol-0.1.0/src/exceptioncontrol/unittests/test_ExceptionControl.py` & `exceptioncontrol-0.1.0.1/src/exceptioncontrol/unittests/test_ExceptionControl.py`

 * *Files identical despite different names*

### Comparing `exceptioncontrol-0.1.0/src/exceptioncontrol/version.py` & `exceptioncontrol-0.1.0.1/src/exceptioncontrol/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #===============================================================================
 """
 """
 
 # Note, when updating this, the docstring in StronglyTypedProperty
 # and in pyproject.toml should also be updated
-__version__ = "0.1.0"
+__version__ = "0.1.0.1"
```

### Comparing `exceptioncontrol-0.1.0/PKG-INFO` & `exceptioncontrol-0.1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: exceptioncontrol
-Version: 0.1.0
+Version: 0.1.0.1
 Summary: Helper class for exception handling
 Home-page: https://gitlab.com/semantik-software/code/python/ExceptionControl
 License: LICENSE
 Keywords: Exception Handling,Debugging
-Author: William McLendon
-Author-email: wcmclen@hotmail.com
-Maintainer: William McLendon
-Maintainer-email: wcmclen@hotmail.com
+Author: William
+Author-email: Semantik-Codeworks@outlook.com
+Maintainer: William
+Maintainer-email: Semantik-Codeworks@outlook.com
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
```

