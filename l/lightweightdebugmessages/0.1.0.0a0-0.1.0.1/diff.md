# Comparing `tmp/lightweightdebugmessages-0.1.0.0a0.tar.gz` & `tmp/lightweightdebugmessages-0.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightweightdebugmessages-0.1.0.0a0.tar", max compression
+gzip compressed data, was "lightweightdebugmessages-0.1.0.1.tar", max compression
```

## Comparing `lightweightdebugmessages-0.1.0.0a0.tar` & `lightweightdebugmessages-0.1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      732 2023-06-23 04:52:57.821341 lightweightdebugmessages-0.1.0.0a0/CHANGELOG.md
--rw-r--r--   0        0        0     1732 2023-05-31 03:25:27.620372 lightweightdebugmessages-0.1.0.0a0/LICENSE
--rw-r--r--   0        0        0     1054 2023-06-23 05:03:31.380099 lightweightdebugmessages-0.1.0.0a0/README.md
--rw-r--r--   0        0        0     1629 2023-06-23 05:11:06.415713 lightweightdebugmessages-0.1.0.0a0/pyproject.toml
--rw-r--r--   0        0        0     5591 2023-06-12 05:18:44.899304 lightweightdebugmessages-0.1.0.0a0/src/lightweightdebugmessages/LightweightDebugMessages.py
--rw-r--r--   0        0        0     2461 2023-06-23 04:52:57.821341 lightweightdebugmessages-0.1.0.0a0/src/lightweightdebugmessages/__init__.py
--rw-r--r--   0        0        0      158 2023-04-26 02:30:20.708024 lightweightdebugmessages-0.1.0.0a0/src/lightweightdebugmessages/unittests/__init__.py
--rw-r--r--   0        0        0     2163 2023-06-12 05:19:41.849282 lightweightdebugmessages-0.1.0.0a0/src/lightweightdebugmessages/unittests/common.py
--rw-r--r--   0        0        0     5998 2023-06-12 05:21:56.179243 lightweightdebugmessages-0.1.0.0a0/src/lightweightdebugmessages/unittests/test_LightweightDebugMessages.py
--rw-r--r--   0        0        0     2460 2023-06-12 05:17:52.439303 lightweightdebugmessages-0.1.0.0a0/src/lightweightdebugmessages/version.py
--rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 lightweightdebugmessages-0.1.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0      828 2023-07-31 00:17:32.001585 lightweightdebugmessages-0.1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1732 2023-05-31 03:25:27.620372 lightweightdebugmessages-0.1.0.1/LICENSE
+-rw-r--r--   0        0        0     1054 2023-06-23 05:03:31.380099 lightweightdebugmessages-0.1.0.1/README.md
+-rw-r--r--   0        0        0     1632 2023-07-31 00:17:07.271589 lightweightdebugmessages-0.1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5591 2023-06-12 05:18:44.899304 lightweightdebugmessages-0.1.0.1/src/lightweightdebugmessages/LightweightDebugMessages.py
+-rw-r--r--   0        0        0     2461 2023-06-23 04:52:57.821341 lightweightdebugmessages-0.1.0.1/src/lightweightdebugmessages/__init__.py
+-rw-r--r--   0        0        0      158 2023-04-26 02:30:20.708024 lightweightdebugmessages-0.1.0.1/src/lightweightdebugmessages/unittests/__init__.py
+-rw-r--r--   0        0        0     2163 2023-06-12 05:19:41.849282 lightweightdebugmessages-0.1.0.1/src/lightweightdebugmessages/unittests/common.py
+-rw-r--r--   0        0        0     5998 2023-06-12 05:21:56.179243 lightweightdebugmessages-0.1.0.1/src/lightweightdebugmessages/unittests/test_LightweightDebugMessages.py
+-rw-r--r--   0        0        0     2462 2023-07-31 00:17:42.471583 lightweightdebugmessages-0.1.0.1/src/lightweightdebugmessages/version.py
+-rw-r--r--   0        0        0     2512 1970-01-01 00:00:00.000000 lightweightdebugmessages-0.1.0.1/PKG-INFO
```

### Comparing `lightweightdebugmessages-0.1.0.0a0/CHANGELOG.md` & `lightweightdebugmessages-0.1.0.1/CHANGELOG.md`

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
+- Minor updates to documentation
+
 
 ## [0.1.0] - 2023-06-12
 ### Added
 ### Changed
 - Rename Debuggable to LightweightDebugMessages
 - Develop documentation for stand-alone package
 - Initial extraction from ConfigParserEnhanced
```

### Comparing `lightweightdebugmessages-0.1.0.0a0/LICENSE` & `lightweightdebugmessages-0.1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lightweightdebugmessages-0.1.0.0a0/README.md` & `lightweightdebugmessages-0.1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `lightweightdebugmessages-0.1.0.0a0/pyproject.toml` & `lightweightdebugmessages-0.1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "lightweightdebugmessages"
 description = "Helper class for exception handling"
-version = "0.1.0.0a"
+version = "0.1.0.1"
 license = "LICENSE"
 readme = "README.md"
 keywords = [
     "Debugging",
     "Logging"
 ]
 repository = "https://gitlab.com/semantik-software/code/python/LightweightDebugMessages"
 documentation = "https://semantik-software.gitlab.io/code/python/LightweightDebugMessages"
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

### Comparing `lightweightdebugmessages-0.1.0.0a0/src/lightweightdebugmessages/LightweightDebugMessages.py` & `lightweightdebugmessages-0.1.0.1/src/lightweightdebugmessages/LightweightDebugMessages.py`

 * *Files identical despite different names*

### Comparing `lightweightdebugmessages-0.1.0.0a0/src/lightweightdebugmessages/__init__.py` & `lightweightdebugmessages-0.1.0.1/src/lightweightdebugmessages/__init__.py`

 * *Files identical despite different names*

### Comparing `lightweightdebugmessages-0.1.0.0a0/src/lightweightdebugmessages/unittests/common.py` & `lightweightdebugmessages-0.1.0.1/src/lightweightdebugmessages/unittests/common.py`

 * *Files identical despite different names*

### Comparing `lightweightdebugmessages-0.1.0.0a0/src/lightweightdebugmessages/unittests/test_LightweightDebugMessages.py` & `lightweightdebugmessages-0.1.0.1/src/lightweightdebugmessages/unittests/test_LightweightDebugMessages.py`

 * *Files identical despite different names*

### Comparing `lightweightdebugmessages-0.1.0.0a0/src/lightweightdebugmessages/version.py` & `lightweightdebugmessages-0.1.0.1/src/lightweightdebugmessages/version.py`

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

### Comparing `lightweightdebugmessages-0.1.0.0a0/PKG-INFO` & `lightweightdebugmessages-0.1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: lightweightdebugmessages
-Version: 0.1.0.0a0
+Version: 0.1.0.1
 Summary: Helper class for exception handling
 Home-page: https://gitlab.com/semantik-software/code/python/LightweightDebugMessages
 License: LICENSE
 Keywords: Debugging,Logging
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

