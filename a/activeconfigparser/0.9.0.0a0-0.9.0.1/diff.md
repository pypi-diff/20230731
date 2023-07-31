# Comparing `tmp/activeconfigparser-0.9.0.0a0.tar.gz` & `tmp/activeconfigparser-0.9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activeconfigparser-0.9.0.0a0.tar", max compression
+gzip compressed data, was "activeconfigparser-0.9.0.1.tar", max compression
```

## Comparing `activeconfigparser-0.9.0.0a0.tar` & `activeconfigparser-0.9.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    17773 2023-06-29 11:08:24.620970 activeconfigparser-0.9.0.0a0/CHANGELOG.md
--rw-r--r--   0        0        0     1732 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/LICENSE
--rw-r--r--   0        0        0     3565 2023-06-29 11:02:00.401110 activeconfigparser-0.9.0.0a0/README.md
--rw-r--r--   0        0        0     1907 2023-06-29 11:09:54.430951 activeconfigparser-0.9.0.0a0/pyproject.toml
--rw-r--r--   0        0        0    75272 2023-06-29 09:53:50.912341 activeconfigparser-0.9.0.0a0/src/activeconfigparser/ActiveConfigParser.py
--rw-r--r--   0        0        0     5186 2023-06-29 11:02:00.401110 activeconfigparser-0.9.0.0a0/src/activeconfigparser/HandlerParameters.py
--rw-r--r--   0        0        0     2559 2023-06-28 01:15:21.993938 activeconfigparser-0.9.0.0a0/src/activeconfigparser/__init__.py
--rw-r--r--   0        0        0      158 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/__init__.py
--rw-r--r--   0        0        0     4416 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/common.py
--rw-r--r--   0        0        0     3111 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/config_test_activeconfigparser.ini
--rw-r--r--   0        0        0      373 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/config_test_activeconfigparser_badkeys.ini
--rw-r--r--   0        0        0      183 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/config_test_activeconfigparser_default.ini
--rw-r--r--   0        0        0      253 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_01.ini
--rw-r--r--   0        0        0      451 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_02.ini
--rw-r--r--   0        0        0      355 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_03a.ini
--rw-r--r--   0        0        0      409 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_03b.ini
--rw-r--r--   0        0        0    88870 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/test_ActiveConfigParser.py
--rw-r--r--   0        0        0     9706 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/test_HandlerParameters.py
--rw-r--r--   0        0        0     2511 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/version.py
--rw-r--r--   0        0        0     5323 1970-01-01 00:00:00.000000 activeconfigparser-0.9.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0    17842 2023-07-31 00:05:49.171704 activeconfigparser-0.9.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1732 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/LICENSE
+-rw-r--r--   0        0        0     3565 2023-06-29 11:02:00.401110 activeconfigparser-0.9.0.1/README.md
+-rw-r--r--   0        0        0     1898 2023-07-31 00:04:41.191715 activeconfigparser-0.9.0.1/pyproject.toml
+-rw-r--r--   0        0        0    75261 2023-07-31 00:00:10.181760 activeconfigparser-0.9.0.1/src/activeconfigparser/ActiveConfigParser.py
+-rw-r--r--   0        0        0     5186 2023-06-29 11:02:00.401110 activeconfigparser-0.9.0.1/src/activeconfigparser/HandlerParameters.py
+-rw-r--r--   0        0        0     2559 2023-06-28 01:15:21.993938 activeconfigparser-0.9.0.1/src/activeconfigparser/__init__.py
+-rw-r--r--   0        0        0      158 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/__init__.py
+-rw-r--r--   0        0        0     4416 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/common.py
+-rw-r--r--   0        0        0     3111 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/config_test_activeconfigparser.ini
+-rw-r--r--   0        0        0      373 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/config_test_activeconfigparser_badkeys.ini
+-rw-r--r--   0        0        0      183 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/config_test_activeconfigparser_default.ini
+-rw-r--r--   0        0        0      253 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_01.ini
+-rw-r--r--   0        0        0      451 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_02.ini
+-rw-r--r--   0        0        0      355 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_03a.ini
+-rw-r--r--   0        0        0      409 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_03b.ini
+-rw-r--r--   0        0        0    88870 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/test_ActiveConfigParser.py
+-rw-r--r--   0        0        0     9706 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/test_HandlerParameters.py
+-rw-r--r--   0        0        0     2511 2023-07-31 00:04:34.321716 activeconfigparser-0.9.0.1/src/activeconfigparser/version.py
+-rw-r--r--   0        0        0     5313 1970-01-01 00:00:00.000000 activeconfigparser-0.9.0.1/PKG-INFO
```

### Comparing `activeconfigparser-0.9.0.0a0/CHANGELOG.md` & `activeconfigparser-0.9.0.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 ### Deprecated
 ### Removed
 ### Fixed
 ### Internal
 ### Security
 -->
 
+## [0.9.0.1] - 2023-07-31
+### Changed
+- Minor documentation updates
+
 
 ## [0.9.0.0] - 2023-06-29
 ### Added
 - Examples
   - Example 01 - Basic example just showing usage
   - Example 02 - Usage example that shows how cyclic dependencies are handled.
   - Example 03 - Shows how we can *extend* ActiveConfigParser to create custom
```

### Comparing `activeconfigparser-0.9.0.0a0/LICENSE` & `activeconfigparser-0.9.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.0a0/README.md` & `activeconfigparser-0.9.0.1/README.md`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.0a0/pyproject.toml` & `activeconfigparser-0.9.0.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "activeconfigparser"
 description = "A tool that extends configparser to enable enhanced processing of .ini files."
-version = "0.9.0.0a"
+version = "0.9.0.1"
 license = "LICENSE"
 readme = "README.md"
 keywords = [
     "Utility",
     "Bash",
     "Configuration",
     "ActiveConfigParser",
     "ConfigParser"
 ]
 repository = "https://gitlab.com/semantik-software/code/python/ActiveConfigParser"
 documentation = "https://semantik-software.gitlab.io/code/python/ActiveConfigParser/"
 authors = [
-    "William McLendon <Semantik-Code@outlook.com>",
+    "William <Semantik-Codeworks@outlook.com>",
 ]
 maintainers = [
-    "William McLendon <Semantik-Code@outlook.com>",
+    "William <Semantik-Codeworks@outlook.com>",
 ]
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Intended Audience :: System Administrators',
     'Intended Audience :: Other Audience',
     'Programming Language :: Python :: 3.6',
```

### Comparing `activeconfigparser-0.9.0.0a0/src/activeconfigparser/ActiveConfigParser.py` & `activeconfigparser-0.9.0.1/src/activeconfigparser/ActiveConfigParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 Todo:
     Determine if we can use the @final decorators (requires Python 3.8).
     If it doesn't hurt older python versions we should use them to indicate
     what methods should not be overridden, not that Python will enforce this
     but it's better than nothing.
 
 :Authors:
-    - William McLendon <Semantik-Code@outlook.com>
+    - William McLendon <Semantik-Codeworks@outlook.com>
 """
 from __future__ import print_function
 
 import configparser
 import inspect
 import io
 import os
@@ -1166,16 +1166,16 @@
                 exceptions for "SERIOUS" events.
         """
         self._validate_parameter(operation, (str))
 
         handler_name = operation
         handler_name = self._apply_transformation_to_operation(handler_name)
 
-        handler_name_private = "_handler_{}".format(handler_name)
-        handler_name_public = "handler_{}".format(handler_name)
+        handler_name_private = f"_handler_{handler_name}"
+        handler_name_public = f"handler_{handler_name}"
 
         handler_public = self._locate_class_method(handler_name_public)
         handler_private = self._locate_class_method(handler_name_private)
 
         if (handler_private[1] is not None) and (handler_public[1] is not None):
             message = "Ambiguous handler name."
             message += " Both `{}` and `{}` exist".format(handler_name_private, handler_name_public)
```

### Comparing `activeconfigparser-0.9.0.0a0/src/activeconfigparser/HandlerParameters.py` & `activeconfigparser-0.9.0.1/src/activeconfigparser/HandlerParameters.py`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.0a0/src/activeconfigparser/__init__.py` & `activeconfigparser-0.9.0.1/src/activeconfigparser/__init__.py`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/common.py` & `activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/common.py`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/config_test_activeconfigparser.ini` & `activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/config_test_activeconfigparser.ini`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/test_ActiveConfigParser.py` & `activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/test_ActiveConfigParser.py`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/test_HandlerParameters.py` & `activeconfigparser-0.9.0.1/src/activeconfigparser/unittests/test_HandlerParameters.py`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.0a0/src/activeconfigparser/version.py` & `activeconfigparser-0.9.0.1/src/activeconfigparser/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,8 +44,8 @@
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #===============================================================================
 """
 """
 
 # Note, when updating this, the docstring in ActiveConfigParser
 # and in pyproject.toml should also be updated
-__version__ = "0.9.0.0"
+__version__ = "0.9.0.1"
```

### Comparing `activeconfigparser-0.9.0.0a0/PKG-INFO` & `activeconfigparser-0.9.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: activeconfigparser
-Version: 0.9.0.0a0
+Version: 0.9.0.1
 Summary: A tool that extends configparser to enable enhanced processing of .ini files.
 Home-page: https://gitlab.com/semantik-software/code/python/ActiveConfigParser
 License: LICENSE
 Keywords: Utility,Bash,Configuration,ActiveConfigParser,ConfigParser
-Author: William McLendon
-Author-email: Semantik-Code@outlook.com
-Maintainer: William McLendon
-Maintainer-email: Semantik-Code@outlook.com
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

