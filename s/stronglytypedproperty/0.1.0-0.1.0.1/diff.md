# Comparing `tmp/stronglytypedproperty-0.1.0.tar.gz` & `tmp/stronglytypedproperty-0.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stronglytypedproperty-0.1.0.tar", max compression
+gzip compressed data, was "stronglytypedproperty-0.1.0.1.tar", max compression
```

## Comparing `stronglytypedproperty-0.1.0.tar` & `stronglytypedproperty-0.1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2587 2023-05-13 01:37:10.087896 stronglytypedproperty-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1732 2023-04-26 02:29:40.278030 stronglytypedproperty-0.1.0/LICENSE
--rw-r--r--   0        0        0     2584 2023-05-13 01:10:40.887988 stronglytypedproperty-0.1.0/README.md
--rw-r--r--   0        0        0     1724 2023-05-13 01:37:10.087896 stronglytypedproperty-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8385 2023-05-12 02:41:09.393153 stronglytypedproperty-0.1.0/src/stronglytypedproperty/StronglyTypedProperty.py
--rw-r--r--   0        0        0     2502 2023-05-05 00:59:50.740247 stronglytypedproperty-0.1.0/src/stronglytypedproperty/__init__.py
--rw-r--r--   0        0        0     2486 2023-05-05 00:59:28.560251 stronglytypedproperty-0.1.0/src/stronglytypedproperty/unittests/__init__.py
--rw-r--r--   0        0        0     2163 2023-04-26 02:29:40.278030 stronglytypedproperty-0.1.0/src/stronglytypedproperty/unittests/common.py
--rw-r--r--   0        0        0    11363 2023-05-12 02:41:09.413153 stronglytypedproperty-0.1.0/src/stronglytypedproperty/unittests/test_StronglyTypedProperty.py
--rw-r--r--   0        0        0     2505 2023-05-13 01:37:10.087896 stronglytypedproperty-0.1.0/src/stronglytypedproperty/version.py
--rw-r--r--   0        0        0     4333 1970-01-01 00:00:00.000000 stronglytypedproperty-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2680 2023-07-31 00:20:55.531552 stronglytypedproperty-0.1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1732 2023-05-13 01:53:37.977839 stronglytypedproperty-0.1.0.1/LICENSE
+-rw-r--r--   0        0        0     2584 2023-05-13 01:54:00.557838 stronglytypedproperty-0.1.0.1/README.md
+-rw-r--r--   0        0        0     1730 2023-07-31 00:21:17.601547 stronglytypedproperty-0.1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8385 2023-05-13 01:54:00.557838 stronglytypedproperty-0.1.0.1/src/stronglytypedproperty/StronglyTypedProperty.py
+-rw-r--r--   0        0        0     2502 2023-05-13 01:54:00.557838 stronglytypedproperty-0.1.0.1/src/stronglytypedproperty/__init__.py
+-rw-r--r--   0        0        0     2486 2023-05-13 01:54:00.557838 stronglytypedproperty-0.1.0.1/src/stronglytypedproperty/unittests/__init__.py
+-rw-r--r--   0        0        0     2163 2023-05-13 01:53:37.977839 stronglytypedproperty-0.1.0.1/src/stronglytypedproperty/unittests/common.py
+-rw-r--r--   0        0        0    11363 2023-05-13 01:54:00.557838 stronglytypedproperty-0.1.0.1/src/stronglytypedproperty/unittests/test_StronglyTypedProperty.py
+-rw-r--r--   0        0        0     2507 2023-07-31 00:20:24.951557 stronglytypedproperty-0.1.0.1/src/stronglytypedproperty/version.py
+-rw-r--r--   0        0        0     4037 1970-01-01 00:00:00.000000 stronglytypedproperty-0.1.0.1/PKG-INFO
```

### Comparing `stronglytypedproperty-0.1.0/CHANGELOG.md` & `stronglytypedproperty-0.1.0.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

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
+- Minor documentation updates
+
 
 ## [0.1.0] - 2023-05-13
 ### Added
 - Initial PyPi release
 - `Example-02` - demonstrates the use of a *validator*
 - Parameter: `validate_on_set` -- this allows disabling of validation checks
   on set for code running in a "release" mode. This will turn off all validation
```

### Comparing `stronglytypedproperty-0.1.0/LICENSE` & `stronglytypedproperty-0.1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stronglytypedproperty-0.1.0/README.md` & `stronglytypedproperty-0.1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `stronglytypedproperty-0.1.0/pyproject.toml` & `stronglytypedproperty-0.1.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "stronglytypedproperty"
 description = "Adds strongly typed property to a class"
-version = "0.1.0"
+version = "0.1.0.1"
 license = "LICENSE"
 readme = "README.md"
 keywords = [
     "Property",
     "Strongly Typed"
 ]
 repository = "https://gitlab.com/semantik-software/code/python/StronglyTypedProperty"
 documentation = "https://semantik-software.gitlab.io/code/python/StronglyTypedProperty"
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

### Comparing `stronglytypedproperty-0.1.0/src/stronglytypedproperty/StronglyTypedProperty.py` & `stronglytypedproperty-0.1.0.1/src/stronglytypedproperty/StronglyTypedProperty.py`

 * *Files identical despite different names*

### Comparing `stronglytypedproperty-0.1.0/src/stronglytypedproperty/__init__.py` & `stronglytypedproperty-0.1.0.1/src/stronglytypedproperty/__init__.py`

 * *Files identical despite different names*

### Comparing `stronglytypedproperty-0.1.0/src/stronglytypedproperty/unittests/__init__.py` & `stronglytypedproperty-0.1.0.1/src/stronglytypedproperty/unittests/__init__.py`

 * *Files identical despite different names*

### Comparing `stronglytypedproperty-0.1.0/src/stronglytypedproperty/unittests/common.py` & `stronglytypedproperty-0.1.0.1/src/stronglytypedproperty/unittests/common.py`

 * *Files identical despite different names*

### Comparing `stronglytypedproperty-0.1.0/src/stronglytypedproperty/unittests/test_StronglyTypedProperty.py` & `stronglytypedproperty-0.1.0.1/src/stronglytypedproperty/unittests/test_StronglyTypedProperty.py`

 * *Files identical despite different names*

### Comparing `stronglytypedproperty-0.1.0/src/stronglytypedproperty/version.py` & `stronglytypedproperty-0.1.0.1/src/stronglytypedproperty/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,8 +44,8 @@
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #===============================================================================
 """
 """
 
 # Note, when updating this, the docstring in StronglyTypedProperty
 # and in pyproject.toml should also be updated
-__version__ = "0.1.0"
+__version__ = "0.1.0.1"
```

### Comparing `stronglytypedproperty-0.1.0/PKG-INFO` & `stronglytypedproperty-0.1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: stronglytypedproperty
-Version: 0.1.0
+Version: 0.1.0.1
 Summary: Adds strongly typed property to a class
 Home-page: https://gitlab.com/semantik-software/code/python/StronglyTypedProperty
 License: LICENSE
 Keywords: Property,Strongly Typed
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
@@ -20,20 +20,14 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Project-URL: Documentation, https://semantik-software.gitlab.io/code/python/StronglyTypedProperty
 Project-URL: Issues, https://gitlab.com/semantik-software/code/python/stronglytypedproperty/-/issues
 Project-URL: Repository, https://gitlab.com/semantik-software/code/python/StronglyTypedProperty
 Description-Content-Type: text/markdown
 
 <!-- GitLab Badges -->
```

