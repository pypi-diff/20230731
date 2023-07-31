# Comparing `tmp/jinjanator_plugins-23.2.0.tar.gz` & `tmp/jinjanator_plugins-23.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Jul 30 10:29:42 2023, max compression
+gzip compressed data, last modified: Mon Jul 31 13:23:07 2023, max compression
```

## Comparing `jinjanator_plugins-23.2.0.tar` & `jinjanator_plugins-23.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1483 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     9133 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/README.md
--rw-r--r--   0        0        0     1872 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/plugin_example/jinjanator_plugin_example.py
--rw-r--r--   0        0        0      599 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/plugin_example/pyproject.toml
--rw-r--r--   0        0        0     1144 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/plugin_example/tests/test_plugin.py
--rw-r--r--   0        0        0     1296 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/plugin_example/tests/test_plugin_discovery.py
--rw-r--r--   0        0        0     1321 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/plugin_example/tests/test_plugin_discovery_entrypoint.py
--rw-r--r--   0        0        0     3066 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/src/jinjanator_plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/src/jinjanator_plugins/py.typed
--rw-r--r--   0        0        0       32 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/.gitignore
--rw-r--r--   0        0        0    11357 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/LICENSE
--rw-r--r--   0        0        0     6352 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/pyproject.toml
--rw-r--r--   0        0        0     8595 2023-07-30 10:29:42.000000 jinjanator_plugins-23.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1645 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0    10862 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/README.md
+-rw-r--r--   0        0        0     1684 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/plugin_example/jinjanator_plugin_example.py
+-rw-r--r--   0        0        0      599 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/plugin_example/pyproject.toml
+-rw-r--r--   0        0        0     1144 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/plugin_example/tests/test_plugin.py
+-rw-r--r--   0        0        0     1296 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/plugin_example/tests/test_plugin_discovery.py
+-rw-r--r--   0        0        0     1321 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/plugin_example/tests/test_plugin_discovery_entrypoint.py
+-rw-r--r--   0        0        0     3066 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/src/jinjanator_plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/src/jinjanator_plugins/py.typed
+-rw-r--r--   0        0        0       32 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/.gitignore
+-rw-r--r--   0        0        0    11357 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/LICENSE
+-rw-r--r--   0        0        0     6351 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/pyproject.toml
+-rw-r--r--   0        0        0     9723 2023-07-31 13:23:07.000000 jinjanator_plugins-23.2.1/PKG-INFO
```

### Comparing `jinjanator_plugins-23.2.0/CHANGELOG.md` & `jinjanator_plugins-23.2.1/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -24,14 +24,21 @@
 This changelog is managed by towncrier and is compiled at release time.
 
 See https://github.com/kpfleming/jinjanator-plugins/blob/main/.github/CONTRIBUTING.md#changelog for details.
 -->
 
 <!-- towncrier release notes start -->
 
+## [23.2.1](https://github.com/kpfleming/jinjanator-plugins/tree/23.2.1) - 2023-07-31
+
+### Additions
+
+- Add documentation for features added in version 23.2.0.
+
+
 ## [23.2.0](https://github.com/kpfleming/jinjanator-plugins/tree/23.2.0) - 2023-07-30
 
 ### Additions
 
 - Added hook for plugins to report their identities.
   [#1](https://github.com/kpfleming/jinjanator-plugins/issues/1)
 - Added three exceptions which Format plugins can raise to indicate problems with options provided to them.
```

### Comparing `jinjanator_plugins-23.2.0/README.md` & `jinjanator_plugins-23.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -121,43 +121,61 @@
 ### jinjanator_plugin_example.py
 
 ```python
 import codecs
 
 from jinjanator_plugins import (
     Format,
+    FormatOptionUnknownError,
+    FormatOptionUnsupportedError,
+    FormatOptionValueError,
     plugin_filters_hook,
     plugin_formats_hook,
+    plugin_identity_hook,
     plugin_tests_hook,
 )
 
 
 def rot13_filter(value):
     return codecs.encode(value, "rot13")
 
 
 def is_len12_test(value):
     return len(value) == 12
 
 
 def spam_format(data_string, options):
-    if options and options[0] == "ham":
+    ham = False
+
+    if options:
+        for option in options:
+            if option == "ham":
+                ham = True
+            else:
+                raise FormatOptionUnknownError(option)
+
+    if ham:
         return {
             "ham": "ham",
             "cheese": "ham and cheese",
             "potatoes": "ham and potatoes",
         }
 
     return {
         "spam": "spam",
         "cheese": "spam and cheese",
         "potatoes": "spam and potatoes",
     }
 
 
+@plugin_identity_hook
+def plugin_identities():
+    return "example"
+
+
 @plugin_filters_hook
 def plugin_filters():
     return {"rot13": rot13_filter}
 
 
 @plugin_tests_hook
 def plugin_tests():
@@ -170,16 +188,18 @@
 ```
 
 Note that the real example makes use of type annotations, but they
 have been removed here for simplicity.
 
 #### Imports
 
-The imports from `jinjanator_plugins` are necessary for the plugin to
-mark the hooks it wishes to use to provide additional features.
+The imports from `jinjanator_plugins` are necessary for the plugin to:
+* Mark the hooks it wishes to use to provide additional features.
+* Construct one (or more) `Format` objects to describe the formats it supports, if any.
+* Raise option-related exceptions from its format function, if any.
 
 #### rot13_filter
 
 A simple filter function which applies the `rot13` transformation to
 the string value it receives.
 
 #### is_len12_test
@@ -190,14 +210,29 @@
 #### spam_format
 
 A simple format function which ignores the content provided (which
 Jinjanator would have read from a data file), and instead returns one
 of two canned responses based on whether the `ham` option has been
 provided by the user.
 
+#### plugin_identities
+
+The hook function which will be called by Jinjanator to allow this
+plugin to identify itself; the `@plugin_identities_hook` decorator
+marks the function so that it will be found.
+
+The function must return a string, which can contain any information
+needed to identify the plugin. This should include the plugin's name
+and version, and can include versions of any packages on which it
+depends.
+
+This string will be included in the output generated by `jinjanate
+--version`, so it should not include any newlines or other formatting
+characters.
+
 #### plugin_filters
 
 The hook function which will be called by Jinjanator to allow this
 plugin to register any filter functions it provides; the
 `@plugin_filters_hook` decorator marks the function so that it will be
 found.
 
@@ -236,14 +271,30 @@
 to Jinjanator, if needed) and the corresponding value being a Format
 object containing a reference to the format function itself and an
 optional list of file suffixes which can be matched to this format
 during format auto-detection.
 
 Note that the function *must* be named `plugin_formats`; it is the
 second part of the 'magic' mechanism mentioned above.
+
+Format functions can accept 'options' to modify their behavior, and
+should raise the exceptions listed below when needed to inform the
+user if one of the provided options does not meet the format's
+requirements.
+
+* `FormatOptionUnknownError` should be raised when a provided option
+  name is not valid.
+
+* `FormatOptionUnsupportedError` should be raised when a provided
+  option is not supported in combination with the other provided
+  options; it should also be raised when options are provided to a
+  format which does not support options.
+
+* `FormatOptionValueError` should be raised when a provided option has
+  a value that is not valid.
 <!-- fancy-readme end -->
 
 ## Chat
 
 If you'd like to chat with the Jinjanator community, join us on
 [Matrix](https://matrix.to/#/#jinjanator:km6g.us)!
```

### Comparing `jinjanator_plugins-23.2.0/plugin_example/jinjanator_plugin_example.py` & `jinjanator_plugins-23.2.1/plugin_example/jinjanator_plugin_example.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,22 +35,19 @@
     ham = False
 
     if options:
         for option in options:
             if option == "ham":
                 ham = True
             elif option == "uns":
-                msg = f"Format option {option} is not supported."
-                raise FormatOptionUnsupportedError(msg)
+                raise FormatOptionUnsupportedError(option)
             elif option == "val":
-                msg = f"Format option {option} has an invalid value."
-                raise FormatOptionValueError(msg)
+                raise FormatOptionValueError(option)
             else:
-                msg = f"Format option {option} is not known"
-                raise FormatOptionUnknownError(msg)
+                raise FormatOptionUnknownError(option)
 
     if ham:
         return {
             "ham": "ham",
             "cheese": "ham and cheese",
             "potatoes": "ham and potatoes",
         }
```

### Comparing `jinjanator_plugins-23.2.0/plugin_example/pyproject.toml` & `jinjanator_plugins-23.2.1/plugin_example/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jinjanator_plugins-23.2.0/plugin_example/tests/test_plugin.py` & `jinjanator_plugins-23.2.1/plugin_example/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `jinjanator_plugins-23.2.0/plugin_example/tests/test_plugin_discovery.py` & `jinjanator_plugins-23.2.1/plugin_example/tests/test_plugin_discovery.py`

 * *Files identical despite different names*

### Comparing `jinjanator_plugins-23.2.0/plugin_example/tests/test_plugin_discovery_entrypoint.py` & `jinjanator_plugins-23.2.1/plugin_example/tests/test_plugin_discovery_entrypoint.py`

 * *Files identical despite different names*

### Comparing `jinjanator_plugins-23.2.0/src/jinjanator_plugins/__init__.py` & `jinjanator_plugins-23.2.1/src/jinjanator_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `jinjanator_plugins-23.2.0/LICENSE` & `jinjanator_plugins-23.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jinjanator_plugins-23.2.0/pyproject.toml` & `jinjanator_plugins-23.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 text = """
 ## Release Information
 """
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "CHANGELOG.md"
 start-after = "<!-- towncrier release notes start -->"
-#pattern = "\n(###.+?\n)## "
+pattern = "\n(###.+?\n)## "
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 text = """
 ---
 [→ Full Changelog](https://github.com/kpfleming/jinjanator-plugins/blob/main/CHANGELOG.md)
 """
```

### Comparing `jinjanator_plugins-23.2.0/PKG-INFO` & `jinjanator_plugins-23.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinjanator-plugins
-Version: 23.2.0
+Version: 23.2.1
 Summary: Package which provides the plugin API for the Jinjanator tool
 Project-URL: Bug Tracker, https://github.com/kpfleming/jinjanator-plugins/issues
 Project-URL: Homepage, https://github.com/kpfleming/jinjanator-plugins
 Author-email: "Kevin P. Fleming" <jinjanator@kevin.km6g.us>
 License: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
@@ -130,43 +130,61 @@
 ### jinjanator_plugin_example.py
 
 ```python
 import codecs
 
 from jinjanator_plugins import (
     Format,
+    FormatOptionUnknownError,
+    FormatOptionUnsupportedError,
+    FormatOptionValueError,
     plugin_filters_hook,
     plugin_formats_hook,
+    plugin_identity_hook,
     plugin_tests_hook,
 )
 
 
 def rot13_filter(value):
     return codecs.encode(value, "rot13")
 
 
 def is_len12_test(value):
     return len(value) == 12
 
 
 def spam_format(data_string, options):
-    if options and options[0] == "ham":
+    ham = False
+
+    if options:
+        for option in options:
+            if option == "ham":
+                ham = True
+            else:
+                raise FormatOptionUnknownError(option)
+
+    if ham:
         return {
             "ham": "ham",
             "cheese": "ham and cheese",
             "potatoes": "ham and potatoes",
         }
 
     return {
         "spam": "spam",
         "cheese": "spam and cheese",
         "potatoes": "spam and potatoes",
     }
 
 
+@plugin_identity_hook
+def plugin_identities():
+    return "example"
+
+
 @plugin_filters_hook
 def plugin_filters():
     return {"rot13": rot13_filter}
 
 
 @plugin_tests_hook
 def plugin_tests():
@@ -179,16 +197,18 @@
 ```
 
 Note that the real example makes use of type annotations, but they
 have been removed here for simplicity.
 
 #### Imports
 
-The imports from `jinjanator_plugins` are necessary for the plugin to
-mark the hooks it wishes to use to provide additional features.
+The imports from `jinjanator_plugins` are necessary for the plugin to:
+* Mark the hooks it wishes to use to provide additional features.
+* Construct one (or more) `Format` objects to describe the formats it supports, if any.
+* Raise option-related exceptions from its format function, if any.
 
 #### rot13_filter
 
 A simple filter function which applies the `rot13` transformation to
 the string value it receives.
 
 #### is_len12_test
@@ -199,14 +219,29 @@
 #### spam_format
 
 A simple format function which ignores the content provided (which
 Jinjanator would have read from a data file), and instead returns one
 of two canned responses based on whether the `ham` option has been
 provided by the user.
 
+#### plugin_identities
+
+The hook function which will be called by Jinjanator to allow this
+plugin to identify itself; the `@plugin_identities_hook` decorator
+marks the function so that it will be found.
+
+The function must return a string, which can contain any information
+needed to identify the plugin. This should include the plugin's name
+and version, and can include versions of any packages on which it
+depends.
+
+This string will be included in the output generated by `jinjanate
+--version`, so it should not include any newlines or other formatting
+characters.
+
 #### plugin_filters
 
 The hook function which will be called by Jinjanator to allow this
 plugin to register any filter functions it provides; the
 `@plugin_filters_hook` decorator marks the function so that it will be
 found.
 
@@ -245,30 +280,31 @@
 to Jinjanator, if needed) and the corresponding value being a Format
 object containing a reference to the format function itself and an
 optional list of file suffixes which can be matched to this format
 during format auto-detection.
 
 Note that the function *must* be named `plugin_formats`; it is the
 second part of the 'magic' mechanism mentioned above.
-## Release Information
-
 
-## [23.2.0](https://github.com/kpfleming/jinjanator-plugins/tree/23.2.0) - 2023-07-30
+Format functions can accept 'options' to modify their behavior, and
+should raise the exceptions listed below when needed to inform the
+user if one of the provided options does not meet the format's
+requirements.
+
+* `FormatOptionUnknownError` should be raised when a provided option
+  name is not valid.
+
+* `FormatOptionUnsupportedError` should be raised when a provided
+  option is not supported in combination with the other provided
+  options; it should also be raised when options are provided to a
+  format which does not support options.
 
+* `FormatOptionValueError` should be raised when a provided option has
+  a value that is not valid.
+## Release Information
 ### Additions
 
-- Added hook for plugins to report their identities.
-  [[#1](https://github.com/kpfleming/jinjanator-plugins/issues/1)](https://github.com/kpfleming/jinjanator-plugins/issues/1)
-- Added three exceptions which Format plugins can raise to indicate problems with options provided to them.
-  [[#2](https://github.com/kpfleming/jinjanator-plugins/issues/2)](https://github.com/kpfleming/jinjanator-plugins/issues/2)
-
-
-### Changes
-
-- Converted tests to proper unit tests.
-
+- Add documentation for features added in version 23.2.0.
 
-## [23.1.0](https://github.com/kpfleming/jinjanator-plugins/tree/23.1.0) - 2023-07-24
 
-Initial release!
 ---
 [→ Full Changelog](https://github.com/kpfleming/jinjanator-plugins/blob/main/CHANGELOG.md)
```

