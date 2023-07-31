# Comparing `tmp/soagen-0.1.1.tar.gz` & `tmp/soagen-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soagen-0.1.1.tar", last modified: Sun Jul 30 14:46:21 2023, max compression
+gzip compressed data, was "soagen-0.1.2.tar", last modified: Mon Jul 31 15:16:20 2023, max compression
```

## Comparing `soagen-0.1.1.tar` & `soagen-0.1.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 14:46:21.692365 soagen-0.1.1/
--rw-rw-rw-   0        0        0       95 2023-07-30 14:43:28.000000 soagen-0.1.1/CHANGELOG.md
--rw-rw-rw-   0        0        0     1064 2023-07-21 10:29:49.000000 soagen-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1408 2023-07-30 14:46:21.692365 soagen-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      466 2023-07-30 08:46:14.000000 soagen-0.1.1/README.md
--rw-rw-rw-   0        0        0     1893 2023-07-29 16:15:31.000000 soagen-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-30 14:46:21.692365 soagen-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-30 14:46:21.645365 soagen-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-30 14:46:21.669365 soagen-0.1.1/src/soagen/
--rw-rw-rw-   0        0        0      477 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/__init__.py
--rw-rw-rw-   0        0        0      870 2023-07-30 13:58:17.000000 soagen-0.1.1/src/soagen/column.py
--rw-rw-rw-   0        0        0     5008 2023-07-30 12:44:09.000000 soagen-0.1.1/src/soagen/config.py
--rw-rw-rw-   0        0        0      952 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/configurable.py
--rw-rw-rw-   0        0        0    19129 2023-07-30 10:56:14.000000 soagen-0.1.1/src/soagen/cpp.py
--rw-rw-rw-   0        0        0      574 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/errors.py
--rw-rw-rw-   0        0        0    10645 2023-07-30 12:51:27.000000 soagen-0.1.1/src/soagen/header_file.py
-drwxrwxrwx   0        0        0        0 2023-07-30 14:46:21.686366 soagen-0.1.1/src/soagen/hpp/
--rw-rw-rw-   0        0        0     5621 2023-07-30 14:42:24.000000 soagen-0.1.1/src/soagen/hpp/.clang-format
--rw-rw-rw-   0        0        0    11287 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/hpp/allocator.hpp
--rw-rw-rw-   0        0        0    31745 2023-07-30 10:23:11.000000 soagen-0.1.1/src/soagen/hpp/column_traits.hpp
-drwxrwxrwx   0        0        0        0 2023-07-30 14:46:21.690366 soagen-0.1.1/src/soagen/hpp/generated/
--rw-rw-rw-   0        0        0     9857 2023-07-30 14:42:25.000000 soagen-0.1.1/src/soagen/hpp/generated/compressed_pair.hpp
--rw-rw-rw-   0        0        0     2935 2023-07-30 14:42:25.000000 soagen-0.1.1/src/soagen/hpp/generated/core.hpp
--rw-rw-rw-   0        0        0     7897 2023-07-30 14:42:25.000000 soagen-0.1.1/src/soagen/hpp/generated/functions.hpp
--rw-rw-rw-   0        0        0    43678 2023-07-30 14:42:27.000000 soagen-0.1.1/src/soagen/hpp/generated/preprocessor.hpp
--rw-rw-rw-   0        0        0      420 2023-07-30 14:40:17.000000 soagen-0.1.1/src/soagen/hpp/generated/version.hpp
--rw-rw-rw-   0        0        0      816 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/hpp/header_end.hpp
--rw-rw-rw-   0        0        0      929 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/hpp/header_start.hpp
--rw-rw-rw-   0        0        0    15165 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/hpp/iterator.hpp
--rw-rw-rw-   0        0        0    24763 2023-07-30 09:59:17.000000 soagen-0.1.1/src/soagen/hpp/meta.hpp
--rw-rw-rw-   0        0        0     5469 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/hpp/mixins.hpp
--rw-rw-rw-   0        0        0     7272 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/hpp/row.hpp
-drwxrwxrwx   0        0        0        0 2023-07-30 14:46:21.690366 soagen-0.1.1/src/soagen/hpp/single/
--rw-rw-rw-   0        0        0   234058 2023-07-30 14:42:44.000000 soagen-0.1.1/src/soagen/hpp/single/soagen.hpp
--rw-rw-rw-   0        0        0      979 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/hpp/soagen.hpp
--rw-rw-rw-   0        0        0    53592 2023-07-30 10:14:59.000000 soagen-0.1.1/src/soagen/hpp/table.hpp
--rw-rw-rw-   0        0        0    41432 2023-07-30 10:23:24.000000 soagen-0.1.1/src/soagen/hpp/table_traits.hpp
--rw-rw-rw-   0        0        0     1067 2023-07-30 13:01:18.000000 soagen-0.1.1/src/soagen/includes.py
--rw-rw-rw-   0        0        0     1103 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/injectors.py
--rw-rw-rw-   0        0        0     3926 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/log.py
--rw-rw-rw-   0        0        0    23113 2023-07-30 14:42:15.000000 soagen-0.1.1/src/soagen/main.py
--rw-rw-rw-   0        0        0     3018 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/metavars.py
--rw-rw-rw-   0        0        0     5174 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/natvis_file.py
--rw-rw-rw-   0        0        0     1971 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/paths.py
--rw-rw-rw-   0        0        0     6128 2023-07-30 10:13:46.000000 soagen-0.1.1/src/soagen/preprocessor.py
--rw-rw-rw-   0        0        0     2494 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/schemas.py
--rw-rw-rw-   0        0        0    66567 2023-07-30 13:58:31.000000 soagen-0.1.1/src/soagen/struct.py
--rw-rw-rw-   0        0        0     2165 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/type_list.py
--rw-rw-rw-   0        0        0     2697 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/utils.py
--rw-rw-rw-   0        0        0     3576 2023-07-30 14:09:00.000000 soagen-0.1.1/src/soagen/variable.py
--rw-rw-rw-   0        0        0      616 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/version.py
--rw-rw-rw-   0        0        0        6 2023-07-30 14:40:17.000000 soagen-0.1.1/src/soagen/version.txt
--rw-rw-rw-   0        0        0    12323 2023-07-29 16:15:31.000000 soagen-0.1.1/src/soagen/writer.py
-drwxrwxrwx   0        0        0        0 2023-07-30 14:46:21.675366 soagen-0.1.1/src/soagen.egg-info/
--rw-rw-rw-   0        0        0     1408 2023-07-30 14:46:21.000000 soagen-0.1.1/src/soagen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1387 2023-07-30 14:46:21.000000 soagen-0.1.1/src/soagen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 14:46:21.000000 soagen-0.1.1/src/soagen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-30 14:46:21.000000 soagen-0.1.1/src/soagen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-07-30 14:46:21.000000 soagen-0.1.1/src/soagen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-30 14:46:21.000000 soagen-0.1.1/src/soagen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-28 06:00:37.000000 soagen-0.1.1/src/soagen.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-07-31 15:16:20.330018 soagen-0.1.2/
+-rw-rw-rw-   0        0        0      128 2023-07-31 15:15:43.000000 soagen-0.1.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1064 2023-07-21 10:29:49.000000 soagen-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1445 2023-07-31 15:16:20.330018 soagen-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2023-07-30 08:46:14.000000 soagen-0.1.2/README.md
+-rw-rw-rw-   0        0        0     1893 2023-07-29 16:15:31.000000 soagen-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-31 15:16:20.330018 soagen-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 15:16:20.287018 soagen-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 15:16:20.308019 soagen-0.1.2/src/soagen/
+-rw-rw-rw-   0        0        0      477 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/__init__.py
+-rw-rw-rw-   0        0        0      870 2023-07-30 13:58:17.000000 soagen-0.1.2/src/soagen/column.py
+-rw-rw-rw-   0        0        0     4923 2023-07-31 13:43:35.000000 soagen-0.1.2/src/soagen/config.py
+-rw-rw-rw-   0        0        0      952 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/configurable.py
+-rw-rw-rw-   0        0        0    19129 2023-07-30 10:56:14.000000 soagen-0.1.2/src/soagen/cpp.py
+-rw-rw-rw-   0        0        0      574 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/errors.py
+-rw-rw-rw-   0        0        0    10586 2023-07-31 14:13:28.000000 soagen-0.1.2/src/soagen/header_file.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:16:20.324019 soagen-0.1.2/src/soagen/hpp/
+-rw-rw-rw-   0        0        0     5621 2023-07-31 15:15:20.000000 soagen-0.1.2/src/soagen/hpp/.clang-format
+-rw-rw-rw-   0        0        0    11287 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/hpp/allocator.hpp
+-rw-rw-rw-   0        0        0    31484 2023-07-31 13:53:03.000000 soagen-0.1.2/src/soagen/hpp/column_traits.hpp
+drwxrwxrwx   0        0        0        0 2023-07-31 15:16:20.328019 soagen-0.1.2/src/soagen/hpp/generated/
+-rw-rw-rw-   0        0        0     9857 2023-07-31 15:15:20.000000 soagen-0.1.2/src/soagen/hpp/generated/compressed_pair.hpp
+-rw-rw-rw-   0        0        0     2935 2023-07-31 15:15:20.000000 soagen-0.1.2/src/soagen/hpp/generated/core.hpp
+-rw-rw-rw-   0        0        0     7897 2023-07-31 15:15:21.000000 soagen-0.1.2/src/soagen/hpp/generated/functions.hpp
+-rw-rw-rw-   0        0        0    43678 2023-07-31 15:15:23.000000 soagen-0.1.2/src/soagen/hpp/generated/preprocessor.hpp
+-rw-rw-rw-   0        0        0      420 2023-07-31 15:15:20.000000 soagen-0.1.2/src/soagen/hpp/generated/version.hpp
+-rw-rw-rw-   0        0        0      816 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/hpp/header_end.hpp
+-rw-rw-rw-   0        0        0      929 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/hpp/header_start.hpp
+-rw-rw-rw-   0        0        0    15153 2023-07-31 14:45:32.000000 soagen-0.1.2/src/soagen/hpp/iterator.hpp
+-rw-rw-rw-   0        0        0    25186 2023-07-31 12:16:29.000000 soagen-0.1.2/src/soagen/hpp/meta.hpp
+-rw-rw-rw-   0        0        0     5469 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/hpp/mixins.hpp
+-rw-rw-rw-   0        0        0     7280 2023-07-31 12:16:29.000000 soagen-0.1.2/src/soagen/hpp/row.hpp
+drwxrwxrwx   0        0        0        0 2023-07-31 15:16:20.328019 soagen-0.1.2/src/soagen/hpp/single/
+-rw-rw-rw-   0        0        0   234186 2023-07-31 15:15:23.000000 soagen-0.1.2/src/soagen/hpp/single/soagen.hpp
+-rw-rw-rw-   0        0        0      979 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/hpp/soagen.hpp
+-rw-rw-rw-   0        0        0    53592 2023-07-30 10:14:59.000000 soagen-0.1.2/src/soagen/hpp/table.hpp
+-rw-rw-rw-   0        0        0    41432 2023-07-30 10:23:24.000000 soagen-0.1.2/src/soagen/hpp/table_traits.hpp
+-rw-rw-rw-   0        0        0     1067 2023-07-30 13:01:18.000000 soagen-0.1.2/src/soagen/includes.py
+-rw-rw-rw-   0        0        0     1103 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/injectors.py
+-rw-rw-rw-   0        0        0     3926 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/log.py
+-rw-rw-rw-   0        0        0    23157 2023-07-31 14:18:44.000000 soagen-0.1.2/src/soagen/main.py
+-rw-rw-rw-   0        0        0     3018 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/metavars.py
+-rw-rw-rw-   0        0        0     5174 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/natvis_file.py
+-rw-rw-rw-   0        0        0     1971 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/paths.py
+-rw-rw-rw-   0        0        0     6128 2023-07-30 10:13:46.000000 soagen-0.1.2/src/soagen/preprocessor.py
+-rw-rw-rw-   0        0        0     2494 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/schemas.py
+-rw-rw-rw-   0        0        0    66634 2023-07-31 14:13:37.000000 soagen-0.1.2/src/soagen/struct.py
+-rw-rw-rw-   0        0        0     2165 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/type_list.py
+-rw-rw-rw-   0        0        0     2697 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/utils.py
+-rw-rw-rw-   0        0        0     3576 2023-07-30 14:09:00.000000 soagen-0.1.2/src/soagen/variable.py
+-rw-rw-rw-   0        0        0      616 2023-07-29 16:15:31.000000 soagen-0.1.2/src/soagen/version.py
+-rw-rw-rw-   0        0        0        6 2023-07-31 15:15:20.000000 soagen-0.1.2/src/soagen/version.txt
+-rw-rw-rw-   0        0        0    12339 2023-07-31 14:15:42.000000 soagen-0.1.2/src/soagen/writer.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:16:20.315019 soagen-0.1.2/src/soagen.egg-info/
+-rw-rw-rw-   0        0        0     1445 2023-07-31 15:16:20.000000 soagen-0.1.2/src/soagen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1387 2023-07-31 15:16:20.000000 soagen-0.1.2/src/soagen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 15:16:20.000000 soagen-0.1.2/src/soagen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-31 15:16:20.000000 soagen-0.1.2/src/soagen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-07-31 15:16:20.000000 soagen-0.1.2/src/soagen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-31 15:16:20.000000 soagen-0.1.2/src/soagen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-28 06:00:37.000000 soagen-0.1.2/src/soagen.egg-info/zip-safe
```

### Comparing `soagen-0.1.1/LICENSE.txt` & `soagen-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/PKG-INFO` & `soagen-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soagen
-Version: 0.1.1
+Version: 0.1.2
 Summary: Struct-of-Arrays generator for C++ projects.
 Author-email: Mark Gillard <mark.gillard@outlook.com.au>
 License: MIT
 Project-URL: Source, https://github.com/marzer/soagen
 Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer
 Keywords: c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of arrays,parallel-arrays,parallel arrays,std::vector
@@ -33,14 +33,18 @@
 <br><br>
 
 [gitter]: https://gitter.im/marzer/community
 [sponsor]: https://github.com/sponsors/marzer
 
 # Changelog
 
+## v0.1.2
+
+-   Minor refactors.
+
 ## v0.1.1
 
 -   Minor refactors.
 
 ## v0.1.0
 
 -   First public release 🎉&#xFE0F;
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: soagen Version: 0.1.1 Summary: Struct-of-Arrays
+Metadata-Version: 2.1 Name: soagen Version: 0.1.2 Summary: Struct-of-Arrays
 generator for C++ projects. Author-email: Mark Gillard
 gillard@outlook.com.au> License: MIT Project-URL: Source, https://github.com/
 marzer/soagen Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer Keywords:
 c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of
 arrays,parallel-arrays,parallel arrays,std::vector Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
@@ -13,9 +13,9 @@
 badge-sponsor.svg)][sponsor] [![Gitter](docs/images/badge-gitter.svg)][gitter]
 
      â¨&#xFE0F; This README is a stub. Please see the HTML documentation:
                       marzer.github.io/soagenâ¨&#xFE0F;
 
 
 [gitter]: https://gitter.im/marzer/community [sponsor]: https://github.com/
-sponsors/marzer # Changelog ## v0.1.1 - Minor refactors. ## v0.1.0 - First
-public release ð&#xFE0F;
+sponsors/marzer # Changelog ## v0.1.2 - Minor refactors. ## v0.1.1 - Minor
+refactors. ## v0.1.0 - First public release ð&#xFE0F;
```

### Comparing `soagen-0.1.1/pyproject.toml` & `soagen-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/column.py` & `soagen-0.1.2/src/soagen/column.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/config.py` & `soagen-0.1.2/src/soagen/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,29 +61,28 @@
                 cfg = toml.loads(utils.read_all_text_from_file(self.path, logger=log.i))
                 self.__dict__.update(Config.__schema.validate(cfg))
             except Exception as ex:
                 raise SchemaError(str(ex), None)
 
             # namespace
             if self.namespace:
-                if self.namespace in (r'std', r'soagen') or self.namespace.startswith(r'std::'):
+                if self.namespace in (r'std', r'soagen', r'soagen::detail') or self.namespace.startswith(r'std::'):
                     raise SchemaError(rf"namespace: '{self.namespace}' is reserved", None)
                 self.meta.push('namespace', self.namespace)
                 self.meta.push('namespace::name', self.namespace)
                 self.meta.push('namespace::start', f'namespace {self.namespace}\n{{')
                 self.meta.push('namespace::end', r'}')
                 self.meta.push('namespace::scope', rf'{self.namespace}::')
             else:
                 log.w(rf'{current_schema_context()}namespace: not set! polluting the global namespace is bad practice')
                 self.meta.push('namespace', '')
                 self.meta.push('namespace::name', '')
                 self.meta.push('namespace::start', '')
                 self.meta.push('namespace::end', '')
                 self.meta.push('namespace::scope', '')
-            self.namespace_macro_alias = re.sub(r'__+', '_', self.namespace.upper().replace('::', '_'))
 
             # injectors for the 'all_X' sections
             self.all_structs = StructInjector(self, self.all_structs)
 
             # structs
             self.structs = [(k, v) for k, v in self.structs.items()]
             for i in range(len(self.structs)):
```

### Comparing `soagen-0.1.1/src/soagen/configurable.py` & `soagen-0.1.2/src/soagen/configurable.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/cpp.py` & `soagen-0.1.2/src/soagen/cpp.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/errors.py` & `soagen-0.1.2/src/soagen/errors.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/header_file.py` & `soagen-0.1.2/src/soagen/header_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,16 +147,16 @@
 
             #ifndef SOAGEN_DOXYGEN
                 #define SOAGEN_DOXYGEN 1
             #endif
             #ifndef SOAGEN_MAKE_NAME
                 #define SOAGEN_MAKE_NAME(...) static_assert(true)
             #endif
-            #ifndef SOAGEN_MAKE_COL
-                #define SOAGEN_MAKE_COL(...) static_assert(true)
+            #ifndef SOAGEN_MAKE_COLUMN
+                #define SOAGEN_MAKE_COLUMN(...) static_assert(true)
             #endif
             #ifndef SOAGEN_NODISCARD
                 #define SOAGEN_NODISCARD
             #endif
             #ifndef SOAGEN_NODISCARD_CTOR
                 #define SOAGEN_NODISCARD_CTOR
             #endif
@@ -218,15 +218,15 @@
         o(
             rf'''
         //{"-"*(120 - o.indent_width - 2)}
         // forward declarations + soagen internal boilerplate
         //{"-"*(120 - o.indent_width - 2)}
         '''
         )
-        with HiddenFromDoxygen(o):
+        with HiddenFromDoxygen(o), ClangFormatOff(o):
             with Namespace(o, self.config.namespace):
                 for struct in self.structs:
                     with MetaScope(self.config.meta_stack, struct.meta):
                         struct.write_forward_declarations(o)
             o()
             with Namespace(o, 'soagen'):
                 for struct in self.structs:
@@ -235,26 +235,25 @@
             o()
             with Namespace(o, 'soagen::detail'):
                 names = set()
                 for struct in self.structs:
                     for col in struct.columns:
                         names.add(col.name)
                 names = sorted(list(names))
-                with ClangFormatOff(o):
-                    for name in names:
-                        sanitized_name = name.replace('::', '_')
-                        pp_define = rf'SOAGEN_NAME_{sanitized_name}'
-                        o(
-                            rf'''
-                        #ifndef {pp_define}
-                            #define {pp_define}
-                            SOAGEN_MAKE_NAME({name});
-                        #endif
-                        '''
-                        )
+                for name in names:
+                    sanitized_name = name.replace('::', '_')
+                    pp_define = rf'SOAGEN_NAME_{sanitized_name}'
+                    o(
+                        rf'''
+                    #ifndef {pp_define}
+                        #define {pp_define}
+                        SOAGEN_MAKE_NAME({name});
+                    #endif
+                    '''
+                    )
                 for struct in self.structs:
                     with MetaScope(self.config.meta_stack, struct.meta):
                         struct.write_soagen_detail_specializations(o)
 
         # header
         if self.header:
             o(
```

### Comparing `soagen-0.1.1/src/soagen/hpp/.clang-format` & `soagen-0.1.2/src/soagen/hpp/.clang-format`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/hpp/allocator.hpp` & `soagen-0.1.2/src/soagen/hpp/allocator.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/hpp/column_traits.hpp` & `soagen-0.1.2/src/soagen/hpp/column_traits.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -725,23 +725,23 @@
 }
 /// @endcond
 
 namespace soagen
 {
 	/// @brief	Traits for a single column of a table.
 	/// @tparam	ValueType	The column's value type.
-	/// @tparam	ParamType	The type used for the column in function parameter contexts (e.g. push_back()).
 	/// @tparam	Align		The minimum memory alignment of the first element in the column.
+	/// @tparam	ParamType	The type used for the column in function parameter contexts (e.g. push_back()).
 	///
 	///	@attention	This class is an implementation detail for the soagen-generated Structure-of-arrays classes.
 	///				You don't need to know anything about it unless you are implementing your own SoA machinery
 	///				without using the soagen generator.
 	template <typename ValueType,
-			  typename ParamType = soagen::param_type<ValueType>,
-			  size_t Align		 = alignof(ValueType)>
+			  size_t Align		 = alignof(ValueType),
+			  typename ParamType = soagen::param_type<ValueType>>
 	struct SOAGEN_EMPTY_BASES column_traits //
 		SOAGEN_HIDDEN_BASE(public detail::column_traits_base<storage_type<ValueType>>)
 	{
 #if SOAGEN_DOXYGEN
 
 		/// @copydoc soagen::storage_type
 		using storage_type = POXY_IMPLEMENTATION_DETAIL(dummy);
@@ -753,14 +753,31 @@
 		/// @brief	The column's value type.
 		using value_type = ValueType;
 		static_assert(!std::is_reference_v<value_type>, "column value_type may not be a reference");
 		static_assert(!std::is_void_v<value_type>, "column value_type may not be void");
 		static_assert(alignof(value_type) == alignof(typename base_traits::storage_type));
 		static_assert(sizeof(value_type) == sizeof(typename base_traits::storage_type));
 
+		/// @brief	The minimum memory alignment of the first element in the column.
+		///
+		/// @note	This is *not* the alignment of each individual element! That is always `alignof(value_type)`.
+		///			This value is referring to the alignment of the allocation for the entire column's buffer region.
+		static constexpr size_t alignment = max(Align, alignof(value_type));
+		static_assert(has_single_bit(alignment), "column alignment must be a power of two");
+
+		/// @brief	The amount of elements to advance to maintain the requested #alignment for this column.
+		///
+		/// @details	The stride size you need to use when iterating through elements of this column such that
+		///				the starting element for each batch would have the same memory alignment as the value specified
+		/// 			for #alignment.
+		///
+		/// @note		Typically you can ignore this; column elements are always aligned correctly according to their
+		///				type. This is for over-alignment scenarios where you need to do things in batches (e.g. SIMD).
+		static constexpr size_t aligned_stride = lcm(alignment, sizeof(value_type)) / sizeof(value_type);
+
 		/// @brief	The type used for the column in lvalue function parameter contexts (e.g. `push_back(const &)`).
 		using param_type = ParamType;
 		static_assert(!std::is_void_v<param_type>, "column param_type may not be void");
 		static_assert(std::is_reference_v<param_type> || !is_cv<param_type>,
 					  "value parameters may not be cv-qualified");
 		static_assert(base_traits::template is_constructible<param_type>);
 
@@ -772,39 +789,22 @@
 		static_assert(base_traits::template is_constructible<rvalue_type>);
 
 		/// @brief	The type used when forwarding #rvalue_type to the backing container (e.g. `table.emplace_back()`)
 		using rvalue_forward_type = forward_type<rvalue_type>;
 
 		/// @brief	The default type for `emplace()` and `emplace_back()` for columns that have a `default` value.
 		using default_emplace_type = make_cref<rvalue_type>;
-
-		/// @brief	The minimum memory alignment of the first element in the column.
-		///
-		/// @note	This is *not* the alignment of each individual element! That is always `alignof(value_type)`.
-		///			This value is referring to the alignment of the allocation for the entire column's buffer region.
-		static constexpr size_t alignment = max(Align, alignof(value_type));
-		static_assert(has_single_bit(alignment), "column alignment must be a power of two");
-
-		/// @brief	The amount of elements to advance to maintain the requested #alignment for this column.
-		///
-		/// @details	The stride size you need to use when iterating through elements of this column such that
-		///				the starting element for each batch would have the same memory alignment as the value specified
-		/// 			for #alignment.
-		///
-		/// @note		Typically you can ignore this; column elements are always aligned correctly according to their
-		///				type. This is for over-alignment scenarios where you need to do things in batches (e.g. SIMD).
-		static constexpr size_t aligned_stride = lcm(alignment, sizeof(value_type)) / sizeof(value_type);
 	};
 
 	/// @brief True if `T` is an instance of #soagen::column_traits.
 	template <typename T>
 	inline constexpr bool is_column_traits = POXY_IMPLEMENTATION_DETAIL(false);
 	/// @cond
-	template <typename ValueType, typename ParamType, size_t Align>
-	inline constexpr bool is_column_traits<column_traits<ValueType, ParamType, Align>> = true;
+	template <typename ValueType, size_t Align, typename ParamType>
+	inline constexpr bool is_column_traits<column_traits<ValueType, Align, ParamType>> = true;
 	template <typename StorageType>
 	inline constexpr bool is_column_traits<detail::column_traits_base<StorageType>> = true;
 	template <typename T>
 	inline constexpr bool is_column_traits<const T> = is_column_traits<T>;
 	template <typename T>
 	inline constexpr bool is_column_traits<volatile T> = is_column_traits<T>;
 	template <typename T>
@@ -814,28 +814,21 @@
 
 /// @cond
 namespace soagen::detail
 {
 	template <typename T>
 	struct to_base_traits_;
 
-	template <typename ValueType, typename ParamType, size_t Align>
-	struct to_base_traits_<column_traits<ValueType, ParamType, Align>>
+	template <typename ValueType, size_t Align, typename ParamType>
+	struct to_base_traits_<column_traits<ValueType, Align, ParamType>>
 	{
 		using type = column_traits_base<storage_type<ValueType>>;
 
-		static_assert(std::is_base_of_v<type, column_traits<ValueType, ParamType, Align>>);
+		static_assert(std::is_base_of_v<type, column_traits<ValueType, Align, ParamType>>);
 	};
 
 	template <typename T>
 	using to_base_traits = typename to_base_traits_<T>::type;
-
-	template <typename ValueType, //
-			  typename ParamType = param_type<ValueType>,
-			  size_t Align		 = alignof(ValueType)>
-	using make_column = soagen::column_traits<ValueType, //
-											  ParamType,
-											  soagen::max(Align, alignof(ValueType))>;
 }
 /// @endcond
 
 #include "header_end.hpp"
```

### Comparing `soagen-0.1.1/src/soagen/hpp/generated/compressed_pair.hpp` & `soagen-0.1.2/src/soagen/hpp/generated/compressed_pair.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/hpp/generated/core.hpp` & `soagen-0.1.2/src/soagen/hpp/generated/core.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/hpp/generated/functions.hpp` & `soagen-0.1.2/src/soagen/hpp/generated/functions.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/hpp/generated/preprocessor.hpp` & `soagen-0.1.2/src/soagen/hpp/generated/preprocessor.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/hpp/header_end.hpp` & `soagen-0.1.2/src/soagen/hpp/header_end.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/hpp/header_start.hpp` & `soagen-0.1.2/src/soagen/hpp/header_start.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/hpp/iterator.hpp` & `soagen-0.1.2/src/soagen/hpp/iterator.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 		{
 			std::add_const_t<remove_cvref<Table>>* table;
 			typename remove_cvref<Table>::difference_type offset;
 		};
 	}
 	/// @endcond
 
-	/// @brief LegacyRandomAccessIterator for soagen-generated table types.
+	/// @brief RandomAccessIterator for soagen-generated table types.
 	template <typename Table, size_t... Columns>
 	class iterator ///
 		SOAGEN_HIDDEN_BASE(protected detail::iterator_storage<remove_cvref<Table>>)
 	{
 	  public:
 		/// @brief Base SoA table type for this iterator.
 		using table_type = remove_cvref<Table>;
@@ -116,18 +116,18 @@
 
 		/// @brief Alias for #row_type.
 		using value_type = row_type;
 
 		/// @brief Alias for #row_type.
 		using reference = row_type;
 
-		/// @brief This iterator type is a LegacyRandomAccessIterator.
+		/// @brief This iterator type is a RandomAccessIterator.
 		using iterator_category = std::random_access_iterator_tag;
 
-#if SOAGEN_CPP == 17
+#if SOAGEN_CPP <= 17
 		using pointer = void;
 #endif
 
 	  private:
 		/// @cond
 
 		using base		= detail::iterator_storage<remove_cvref<Table>>;
```

### Comparing `soagen-0.1.1/src/soagen/hpp/meta.hpp` & `soagen-0.1.2/src/soagen/hpp/meta.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -39,52 +39,55 @@
 	#define SOAGEN_MAKE_NAME(Name)                                                                                     \
                                                                                                                        \
 		struct name_constant_##Name                                                                                    \
 		{                                                                                                              \
 			static constexpr const char value[] = #Name;                                                               \
 		};                                                                                                             \
                                                                                                                        \
-		template <typename Ref>                                                                                        \
-		struct named_ref_##Name                                                                                        \
+		template <typename T, template <typename> typename Transformation = soagen::identity_type>                     \
+		struct named_member_##Name                                                                                     \
 		{                                                                                                              \
-			Ref Name;                                                                                                  \
+			Transformation<T> Name;                                                                                    \
                                                                                                                        \
 		  protected:                                                                                                   \
 			SOAGEN_PURE_INLINE_GETTER                                                                                  \
-			constexpr Ref get_ref_impl() const noexcept                                                                \
+			constexpr decltype(auto) get_named_member() const noexcept                                                 \
 			{                                                                                                          \
-				return static_cast<Ref>(Name);                                                                         \
+				if constexpr (std::is_reference_v<Transformation<T>>)                                                  \
+					return static_cast<Transformation<T>>(Name);                                                       \
+				else                                                                                                   \
+					return Name;                                                                                       \
 			}                                                                                                          \
 		}
 #endif
 
-#ifndef SOAGEN_MAKE_COL
-	#define SOAGEN_MAKE_COL(Table, Column, Name)                                                                       \
+#ifndef SOAGEN_MAKE_COLUMN
+	#define SOAGEN_MAKE_COLUMN(Table, Column, Name)                                                                    \
 		template <>                                                                                                    \
-		struct col_name_<Table, Column> : name_constant_##Name                                                         \
+		struct column_name_<Table, Column> : name_constant_##Name                                                      \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
 		struct col_ref_<Table&, Column>                                                                                \
-			: named_ref_##Name<std::add_lvalue_reference_t<soagen::value_type<Table, Column>>>                         \
+			: named_member_##Name<std::add_lvalue_reference_t<soagen::value_type<Table, Column>>>                      \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
 		struct col_ref_<Table&&, Column>                                                                               \
-			: named_ref_##Name<std::add_rvalue_reference_t<soagen::value_type<Table, Column>>>                         \
+			: named_member_##Name<std::add_rvalue_reference_t<soagen::value_type<Table, Column>>>                      \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
 		struct col_ref_<const Table&, Column>                                                                          \
-			: named_ref_##Name<std::add_lvalue_reference_t<std::add_const_t<soagen::value_type<Table, Column>>>>       \
+			: named_member_##Name<std::add_lvalue_reference_t<std::add_const_t<soagen::value_type<Table, Column>>>>    \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
 		struct col_ref_<const Table&&, Column>                                                                         \
-			: named_ref_##Name<std::add_rvalue_reference_t<std::add_const_t<soagen::value_type<Table, Column>>>>       \
+			: named_member_##Name<std::add_rvalue_reference_t<std::add_const_t<soagen::value_type<Table, Column>>>>    \
 		{}
 #endif
 
 namespace soagen
 {
 	/// @brief	Equivalent to C+20's std::remove_cvref_t.
 	template <typename T>
@@ -94,14 +97,18 @@
 	template <typename T>
 	using make_cref = std::add_lvalue_reference_t<std::add_const_t<std::remove_reference_t<T>>>;
 
 	/// @brief	Makes `T` into `T&` if `T` was not already a reference.
 	template <typename T>
 	using coerce_ref = std::conditional_t<std::is_reference_v<T>, T, std::add_lvalue_reference_t<T>>;
 
+	/// @brief	The identity type transformation.
+	template <typename T>
+	using identity_type = T;
+
 	/// @brief	True if `T` is `const` or `volatile` qualified.
 	template <typename T>
 	inline constexpr bool is_cv = !std::is_same_v<std::remove_cv_t<T>, T>;
 
 	/// @brief	True if `T` is (or is a reference to something that is) `const` or `volatile` qualified.
 	template <typename T>
 	inline constexpr bool is_cvref = !std::is_same_v<remove_cvref<T>, T>;
@@ -585,15 +592,15 @@
 		}
 	}
 
 	/// @cond
 	namespace detail
 	{
 		template <typename Table, size_t ColumnIndex>
-		struct col_name_;
+		struct column_name_;
 		template <typename Table, size_t ColumnIndex>
 		struct col_ref_;
 
 		template <typename A, typename B>
 		inline constexpr bool same_table_type =
 			std::is_same_v<table_type<remove_cvref<A>>, table_type<remove_cvref<B>>>;
 	}
```

### Comparing `soagen-0.1.1/src/soagen/hpp/mixins.hpp` & `soagen-0.1.2/src/soagen/hpp/mixins.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/hpp/row.hpp` & `soagen-0.1.2/src/soagen/hpp/row.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 
 		template <size_t Column>
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr decltype(auto) column() const noexcept
 		{
 			static_assert(Column < table_traits_type<remove_cvref<Table>>::column_count, "column index out of range");
 
-			return detail::col_ref_<Table, Column>::get_ref_impl();
+			return detail::col_ref_<Table, Column>::get_named_member();
 		}
 
 		// tuple protocol:
 
 		template <size_t Member>
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr decltype(auto) get() const noexcept
 		{
 			static_assert(Member < sizeof...(Columns), "member index out of range");
 
-			return type_at_index<Member, detail::col_ref_<Table, Columns>...>::get_ref_impl();
+			return type_at_index<Member, detail::col_ref_<Table, Columns>...>::get_named_member();
 		}
 
 		/// @name Equality
 		/// @availability These operators are only available when all the column types are equality-comparable.
 		/// @{
 
 		/// @brief Returns true if all of the elements in two rows are equal.
```

### Comparing `soagen-0.1.1/src/soagen/hpp/single/soagen.hpp` & `soagen-0.1.2/src/soagen/hpp/single/soagen.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 //----------------------------------------------------------------------------------------------------------------------
 //
-// soagen.hpp v0.1.1
+// soagen.hpp v0.1.2
 // https://github.com/marzer/soagen
 // SPDX-License-Identifier: MIT
 //
 //----------------------------------------------------------------------------------------------------------------------
 //     !!!!! THIS FILE WAS ASSEMBLED FROM MULTIPLE HEADER FILES BY A SCRIPT - PLEASE DON'T EDIT IT DIRECTLY !!!!!
 //----------------------------------------------------------------------------------------------------------------------
 //
 // MIT License
-//
+// 
 // Copyright (c) Mark Gillard
-//
+// 
 // Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 // documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 // rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to
 // permit persons to whom the Software is furnished to do so, subject to the following conditions:
-//
+// 
 // The above copyright notice and this permission notice shall be included in all copies or substantial portions of the
 // Software.
-//
+// 
 // THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
 // WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 // COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 // OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 //
 //----------------------------------------------------------------------------------------------------------------------
 #ifndef SOAGEN_HPP
 #define SOAGEN_HPP
 
 //********  generated/version.hpp  *************************************************************************************
 
-#define SOAGEN_VERSION_MAJOR  0
-#define SOAGEN_VERSION_MINOR  1
-#define SOAGEN_VERSION_PATCH  1
-#define SOAGEN_VERSION_STRING "0.1.1"
+#define SOAGEN_VERSION_MAJOR 0
+#define SOAGEN_VERSION_MINOR 1
+#define SOAGEN_VERSION_PATCH 2
+#define SOAGEN_VERSION_STRING "0.1.2"
 
 //********  generated/preprocessor.hpp  ********************************************************************************
 
 #ifndef SOAGEN_CPP
 	#ifdef _MSVC_LANG
 		#if _MSVC_LANG > __cplusplus
 			#define SOAGEN_CPP _MSVC_LANG
@@ -1200,52 +1200,55 @@
 	#define SOAGEN_MAKE_NAME(Name)                                                                                     \
                                                                                                                        \
 		struct name_constant_##Name                                                                                    \
 		{                                                                                                              \
 			static constexpr const char value[] = #Name;                                                               \
 		};                                                                                                             \
                                                                                                                        \
-		template <typename Ref>                                                                                        \
-		struct named_ref_##Name                                                                                        \
+		template <typename T, template <typename> typename Transformation = soagen::identity_type>                     \
+		struct named_member_##Name                                                                                     \
 		{                                                                                                              \
-			Ref Name;                                                                                                  \
+			Transformation<T> Name;                                                                                    \
                                                                                                                        \
 		  protected:                                                                                                   \
 			SOAGEN_PURE_INLINE_GETTER                                                                                  \
-			constexpr Ref get_ref_impl() const noexcept                                                                \
+			constexpr decltype(auto) get_named_member() const noexcept                                                 \
 			{                                                                                                          \
-				return static_cast<Ref>(Name);                                                                         \
+				if constexpr (std::is_reference_v<Transformation<T>>)                                                  \
+					return static_cast<Transformation<T>>(Name);                                                       \
+				else                                                                                                   \
+					return Name;                                                                                       \
 			}                                                                                                          \
 		}
 #endif
 
-#ifndef SOAGEN_MAKE_COL
-	#define SOAGEN_MAKE_COL(Table, Column, Name)                                                                       \
+#ifndef SOAGEN_MAKE_COLUMN
+	#define SOAGEN_MAKE_COLUMN(Table, Column, Name)                                                                    \
 		template <>                                                                                                    \
-		struct col_name_<Table, Column> : name_constant_##Name                                                         \
+		struct column_name_<Table, Column> : name_constant_##Name                                                      \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
 		struct col_ref_<Table&, Column>                                                                                \
-			: named_ref_##Name<std::add_lvalue_reference_t<soagen::value_type<Table, Column>>>                         \
+			: named_member_##Name<std::add_lvalue_reference_t<soagen::value_type<Table, Column>>>                      \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
 		struct col_ref_<Table&&, Column>                                                                               \
-			: named_ref_##Name<std::add_rvalue_reference_t<soagen::value_type<Table, Column>>>                         \
+			: named_member_##Name<std::add_rvalue_reference_t<soagen::value_type<Table, Column>>>                      \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
 		struct col_ref_<const Table&, Column>                                                                          \
-			: named_ref_##Name<std::add_lvalue_reference_t<std::add_const_t<soagen::value_type<Table, Column>>>>       \
+			: named_member_##Name<std::add_lvalue_reference_t<std::add_const_t<soagen::value_type<Table, Column>>>>    \
 		{};                                                                                                            \
                                                                                                                        \
 		template <>                                                                                                    \
 		struct col_ref_<const Table&&, Column>                                                                         \
-			: named_ref_##Name<std::add_rvalue_reference_t<std::add_const_t<soagen::value_type<Table, Column>>>>       \
+			: named_member_##Name<std::add_rvalue_reference_t<std::add_const_t<soagen::value_type<Table, Column>>>>    \
 		{}
 #endif
 
 namespace soagen
 {
 	template <typename T>
 	using remove_cvref = std::remove_cv_t<std::remove_reference_t<T>>;
@@ -1253,14 +1256,17 @@
 	template <typename T>
 	using make_cref = std::add_lvalue_reference_t<std::add_const_t<std::remove_reference_t<T>>>;
 
 	template <typename T>
 	using coerce_ref = std::conditional_t<std::is_reference_v<T>, T, std::add_lvalue_reference_t<T>>;
 
 	template <typename T>
+	using identity_type = T;
+
+	template <typename T>
 	inline constexpr bool is_cv = !std::is_same_v<std::remove_cv_t<T>, T>;
 
 	template <typename T>
 	inline constexpr bool is_cvref = !std::is_same_v<remove_cvref<T>, T>;
 
 	template <typename T>
 	inline constexpr bool is_integer = std::is_integral_v<T> && !std::is_same_v<T, bool>;
@@ -1646,15 +1652,15 @@
 			return static_cast<Func&&>(func)(static_cast<Arg&&>(arg));
 		}
 	}
 
 	namespace detail
 	{
 		template <typename Table, size_t ColumnIndex>
-		struct col_name_;
+		struct column_name_;
 		template <typename Table, size_t ColumnIndex>
 		struct col_ref_;
 
 		template <typename A, typename B>
 		inline constexpr bool same_table_type =
 			std::is_same_v<table_type<remove_cvref<A>>, table_type<remove_cvref<B>>>;
 	}
@@ -1723,26 +1729,26 @@
 
 		template <size_t Column>
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr decltype(auto) column() const noexcept
 		{
 			static_assert(Column < table_traits_type<remove_cvref<Table>>::column_count, "column index out of range");
 
-			return detail::col_ref_<Table, Column>::get_ref_impl();
+			return detail::col_ref_<Table, Column>::get_named_member();
 		}
 
 		// tuple protocol:
 
 		template <size_t Member>
 		SOAGEN_PURE_INLINE_GETTER
 		constexpr decltype(auto) get() const noexcept
 		{
 			static_assert(Member < sizeof...(Columns), "member index out of range");
 
-			return type_at_index<Member, detail::col_ref_<Table, Columns>...>::get_ref_impl();
+			return type_at_index<Member, detail::col_ref_<Table, Columns>...>::get_named_member();
 		}
 
 		SOAGEN_CONSTRAINED_TEMPLATE((detail::same_table_type<Table, T>
 									 && table_traits_type<remove_cvref<Table>>::all_equality_comparable),
 									typename T)
 		SOAGEN_NODISCARD
 		friend constexpr bool operator==(const row& lhs, const row<T, Columns...>& rhs) //
@@ -3451,52 +3457,52 @@
 		}
 	};
 }
 
 namespace soagen
 {
 	template <typename ValueType,
-			  typename ParamType = soagen::param_type<ValueType>,
-			  size_t Align		 = alignof(ValueType)>
+			  size_t Align		 = alignof(ValueType),
+			  typename ParamType = soagen::param_type<ValueType>>
 	struct SOAGEN_EMPTY_BASES column_traits //
 		SOAGEN_HIDDEN_BASE(public detail::column_traits_base<storage_type<ValueType>>)
 	{
 		using base_traits = detail::column_traits_base<storage_type<ValueType>>;
 
 		using value_type = ValueType;
 		static_assert(!std::is_reference_v<value_type>, "column value_type may not be a reference");
 		static_assert(!std::is_void_v<value_type>, "column value_type may not be void");
 		static_assert(alignof(value_type) == alignof(typename base_traits::storage_type));
 		static_assert(sizeof(value_type) == sizeof(typename base_traits::storage_type));
 
+		static constexpr size_t alignment = max(Align, alignof(value_type));
+		static_assert(has_single_bit(alignment), "column alignment must be a power of two");
+
+		static constexpr size_t aligned_stride = lcm(alignment, sizeof(value_type)) / sizeof(value_type);
+
 		using param_type = ParamType;
 		static_assert(!std::is_void_v<param_type>, "column param_type may not be void");
 		static_assert(std::is_reference_v<param_type> || !is_cv<param_type>,
 					  "value parameters may not be cv-qualified");
 		static_assert(base_traits::template is_constructible<param_type>);
 
 		using param_forward_type = forward_type<param_type>;
 
 		using rvalue_type = soagen::rvalue_type<param_type>;
 		static_assert(base_traits::template is_constructible<rvalue_type>);
 
 		using rvalue_forward_type = forward_type<rvalue_type>;
 
 		using default_emplace_type = make_cref<rvalue_type>;
-
-		static constexpr size_t alignment = max(Align, alignof(value_type));
-		static_assert(has_single_bit(alignment), "column alignment must be a power of two");
-
-		static constexpr size_t aligned_stride = lcm(alignment, sizeof(value_type)) / sizeof(value_type);
 	};
 
 	template <typename T>
 	inline constexpr bool is_column_traits = POXY_IMPLEMENTATION_DETAIL(false);
-	template <typename ValueType, typename ParamType, size_t Align>
-	inline constexpr bool is_column_traits<column_traits<ValueType, ParamType, Align>> = true;
+	template <typename ValueType, size_t Align, typename ParamType>
+	inline constexpr bool is_column_traits<column_traits<ValueType, Align, ParamType>> = true;
 	template <typename StorageType>
 	inline constexpr bool is_column_traits<detail::column_traits_base<StorageType>> = true;
 	template <typename T>
 	inline constexpr bool is_column_traits<const T> = is_column_traits<T>;
 	template <typename T>
 	inline constexpr bool is_column_traits<volatile T> = is_column_traits<T>;
 	template <typename T>
@@ -3504,31 +3510,24 @@
 }
 
 namespace soagen::detail
 {
 	template <typename T>
 	struct to_base_traits_;
 
-	template <typename ValueType, typename ParamType, size_t Align>
-	struct to_base_traits_<column_traits<ValueType, ParamType, Align>>
+	template <typename ValueType, size_t Align, typename ParamType>
+	struct to_base_traits_<column_traits<ValueType, Align, ParamType>>
 	{
 		using type = column_traits_base<storage_type<ValueType>>;
 
-		static_assert(std::is_base_of_v<type, column_traits<ValueType, ParamType, Align>>);
+		static_assert(std::is_base_of_v<type, column_traits<ValueType, Align, ParamType>>);
 	};
 
 	template <typename T>
 	using to_base_traits = typename to_base_traits_<T>::type;
-
-	template <typename ValueType, //
-			  typename ParamType = param_type<ValueType>,
-			  size_t Align		 = alignof(ValueType)>
-	using make_column = soagen::column_traits<ValueType, //
-											  ParamType,
-											  soagen::max(Align, alignof(ValueType))>;
 }
 
 #if SOAGEN_ALWAYS_OPTIMIZE
 	#if SOAGEN_MSVC
 		#pragma strict_gs_check(pop)
 		#pragma runtime_checks("", restore)
 		#pragma optimize("", on)
@@ -6507,15 +6506,16 @@
 		struct iterator_storage
 		{
 			std::add_const_t<remove_cvref<Table>>* table;
 			typename remove_cvref<Table>::difference_type offset;
 		};
 	}
 	template <typename Table, size_t... Columns>
-	class iterator SOAGEN_HIDDEN_BASE(protected detail::iterator_storage<remove_cvref<Table>>)
+	class iterator
+		SOAGEN_HIDDEN_BASE(protected detail::iterator_storage<remove_cvref<Table>>)
 	{
 	  public:
 		using table_type = remove_cvref<Table>;
 		static_assert(is_soa<table_type>, "soagen iterators are for use with soagen-generated SoA table types.");
 
 		using table_ref = Table;
 		static_assert(std::is_reference_v<table_ref>,
@@ -6529,19 +6529,20 @@
 
 		using value_type = row_type;
 
 		using reference = row_type;
 
 		using iterator_category = std::random_access_iterator_tag;
 
-#if SOAGEN_CPP == 17
+#if SOAGEN_CPP <= 17
 		using pointer = void;
 #endif
 
 	  private:
+
 		using base		= detail::iterator_storage<remove_cvref<Table>>;
 		using table_ptr = std::add_pointer_t<std::remove_reference_t<Table>>;
 
 		template <typename, size_t...>
 		friend class soagen::iterator;
 
 		SOAGEN_NODISCARD_CTOR
```

### Comparing `soagen-0.1.1/src/soagen/hpp/soagen.hpp` & `soagen-0.1.2/src/soagen/hpp/soagen.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/hpp/table.hpp` & `soagen-0.1.2/src/soagen/hpp/table.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/hpp/table_traits.hpp` & `soagen-0.1.2/src/soagen/hpp/table_traits.hpp`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/includes.py` & `soagen-0.1.2/src/soagen/includes.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/injectors.py` & `soagen-0.1.2/src/soagen/injectors.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/log.py` & `soagen-0.1.2/src/soagen/log.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/main.py` & `soagen-0.1.2/src/soagen/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -174,15 +174,15 @@
                         r'*.dox',
                         r'*.toml',
                         r'*.natvis',
                         r'meson.build',
                     ),
                     recursive=recursive,
                 ):
-                    if str(file).find('.egg-info') != -1 or file.name.lower.find('changelog') != -1:
+                    if str(file).find('.egg-info') != -1 or file.name.lower().find('changelog') != -1:
                         continue
                     text = utils.read_all_text_from_file(file, logger=log.d)
                     new_text = matcher.sub(VERSION_STRING, text)
                     new_text = matcher_v.sub(lambda m: m[1] + VERSION_STRING, new_text)
                     if text != new_text:
                         log.i(rf'Writing updated version numbers in {file}')
                         with open(file, 'w', encoding='utf-8', newline='\n') as f:
@@ -235,18 +235,14 @@
         soagen_hpp_in = Path(paths.HPP, 'soagen.hpp')
         soagen_hpp_out = Path(paths.HPP_SINGLE, 'soagen.hpp')
         text = str(Preprocessor(soagen_hpp_in))
         text = utils.replace_metavar(r'version', VERSION_STRING, text)
         license = utils.read_all_text_from_file(paths.REPOSITORY / r'LICENSE.txt', log.i).replace('\r\n', '\n').strip()
         license = '\n// '.join(utils.reflow_text(license, line_length=117).split('\n'))
         text = utils.replace_metavar(r'license', license, text)
-        try:
-            text = utils.clang_format(text, cwd=soagen_hpp_in.parent)
-        except:
-            pass
         log.i(rf'Writing {soagen_hpp_out}')
         os.makedirs(str(paths.HPP_SINGLE), exist_ok=True)
         with open(soagen_hpp_out, 'w', encoding='utf-8', newline='\n') as f:
             f.write(text)
 
     # re-run soagen itself on the examples and tests
     if update_examples and paths.EXAMPLES.exists():
@@ -426,24 +422,27 @@
         done_work = True
         args.install: Path
         if not args.install.exists() or not args.install.is_dir():
             log.e(rf"--install: path '{args.install}' did not exist or was not a directory")
         log.i(rf"Copying soagen.hpp to {args.install.resolve()}")
         utils.copy_file(paths.HPP_SINGLE / r'soagen.hpp', args.install)
 
-    configs = []
-    for p in args.configs:
-        if p.find('*') != -1:
-            configs = configs + [f for f in Path('.').glob(p) if f.is_file()]
+    configs = set()
+    for config in args.configs:
+        if config == '.':
+            config = '*.toml'
+        if config.find('*') != -1:
+            configs.update([f for f in Path('.').glob(config) if f.is_file()])
         else:
-            p = Path(p)
-            if not p.exists() or not p.is_file():
-                log.e(rf"configs: '{p}' did not exist or was not a file")
-            configs.append(p)
-    configs.sort()
+            config = Path(config)
+            if config not in configs:
+                if not config.exists() or not config.is_file():
+                    log.e(rf"configs: '{config}' did not exist or was not a file")
+                configs.add(config)
+    configs = sorted(configs)
     if args.bug_report_internal:
         os.makedirs(str(paths.BUG_REPORT_INPUTS), exist_ok=True)
         for f in configs:
             utils.copy_file(f, paths.BUG_REPORT_INPUTS, log.i)
     configs = [Config(f) for f in configs]
     done_work = done_work or bool(configs)
```

### Comparing `soagen-0.1.1/src/soagen/metavars.py` & `soagen-0.1.2/src/soagen/metavars.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/natvis_file.py` & `soagen-0.1.2/src/soagen/natvis_file.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/paths.py` & `soagen-0.1.2/src/soagen/paths.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/preprocessor.py` & `soagen-0.1.2/src/soagen/preprocessor.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/schemas.py` & `soagen-0.1.2/src/soagen/schemas.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/struct.py` & `soagen-0.1.2/src/soagen/struct.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,21 +187,21 @@
             max_length = max(len(col.name), max_length)
         with StringIO() as buf:
             buf.write('table_traits<\n')
             for i in range(len(self.columns)):
                 if i:
                     buf.write(f',\n')
                 col = self.columns[i]
-                buf.write(f'{o.indent_str*4}/* {col.name:>{max_length}} */ make_column<{col.type}')
-                if col.param_type:
-                    buf.write(rf', {col.param_type}')
+                buf.write(f'{o.indent_str*4}/* {col.name:>{max_length}} */ column_traits<{col.type}')
                 if col.alignment > 0:
+                    buf.write(rf', soagen::max(size_t{{ {col.alignment} }}, alignof({col.type}))')
+                if col.param_type:
                     if not col.param_type:
-                        buf.write(rf', param_type<{col.type}>')
-                    buf.write(rf', {col.alignment}')
+                        buf.write(rf', alignof({col.type})')
+                    buf.write(rf', {col.param_type}')
                 buf.write(rf'>')
             buf.write(rf'>')
             o(
                 rf'''
             template <>
             struct table_traits_type_<{self.qualified_name}>
             {{
@@ -213,15 +213,15 @@
             {{
                 using type = {self.allocator};
             }};
             '''
             )
 
             for col in self.columns:
-                o(rf'SOAGEN_MAKE_COL({self.qualified_name}, {col.index}, {col.name});')
+                o(rf'SOAGEN_MAKE_COLUMN({self.qualified_name}, {col.index}, {col.name});')
 
         o(
             rf'''
         template <>
         struct table_type_<{self.qualified_name}>
         {{
             using type = table<table_traits_type<{self.qualified_name}>, {self.allocator}>;
@@ -394,16 +394,16 @@
 
                     if o.doxygen:
                         o('#endif')
 
                     o(
                         rf'''
 
-                    {doxygen(r"@brief Gets the name of the specified column as a string.")}
-                    template <size_type Column> static constexpr auto& column_name = soagen::detail::col_name_<{self.name}, Column>::value;
+                    {doxygen(r"@brief Gets the name of the specified column as a null-terminated string.")}
+                    template <size_type Column> static constexpr auto& column_name = soagen::detail::column_name_<{self.name}, Column>::value;
 
                     {self.header}
 
                     '''
                     )
 
                 for access in (r'public', r'protected', r'private'):
```

### Comparing `soagen-0.1.1/src/soagen/type_list.py` & `soagen-0.1.2/src/soagen/type_list.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/utils.py` & `soagen-0.1.2/src/soagen/utils.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/variable.py` & `soagen-0.1.2/src/soagen/variable.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/version.py` & `soagen-0.1.2/src/soagen/version.py`

 * *Files identical despite different names*

### Comparing `soagen-0.1.1/src/soagen/writer.py` & `soagen-0.1.2/src/soagen/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -366,21 +366,23 @@
             r'''
         #endif'''
         )
 
 
 class ClangFormatOff(WriterBlockBase):
     def __enter__(self):
-        if self.writer.doxygen:
-            self.writer('// clang-format off')
+        self.writer()
+        self.writer('// clang-format off')
+        self.writer()
         return self
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
-        if self.writer.doxygen:
-            self.writer('// clang-format on')
+        self.writer()
+        self.writer('// clang-format on')
+        self.writer()
 
 
 __all__ = [
     r'WriterBlockBase',
     r'Writer',
     r'Indent',
     r'Namespace',
```

### Comparing `soagen-0.1.1/src/soagen.egg-info/PKG-INFO` & `soagen-0.1.2/src/soagen.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soagen
-Version: 0.1.1
+Version: 0.1.2
 Summary: Struct-of-Arrays generator for C++ projects.
 Author-email: Mark Gillard <mark.gillard@outlook.com.au>
 License: MIT
 Project-URL: Source, https://github.com/marzer/soagen
 Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer
 Keywords: c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of arrays,parallel-arrays,parallel arrays,std::vector
@@ -33,14 +33,18 @@
 <br><br>
 
 [gitter]: https://gitter.im/marzer/community
 [sponsor]: https://github.com/sponsors/marzer
 
 # Changelog
 
+## v0.1.2
+
+-   Minor refactors.
+
 ## v0.1.1
 
 -   Minor refactors.
 
 ## v0.1.0
 
 -   First public release 🎉&#xFE0F;
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: soagen Version: 0.1.1 Summary: Struct-of-Arrays
+Metadata-Version: 2.1 Name: soagen Version: 0.1.2 Summary: Struct-of-Arrays
 generator for C++ projects. Author-email: Mark Gillard
 gillard@outlook.com.au> License: MIT Project-URL: Source, https://github.com/
 marzer/soagen Project-URL: Tracker, https://github.com/marzer/soagen/issues
 Project-URL: Funding, https://github.com/sponsors/marzer Keywords:
 c++,soa,struct-of-arrays,structure-of-arrays,struct of arrays,structure of
 arrays,parallel-arrays,parallel arrays,std::vector Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
@@ -13,9 +13,9 @@
 badge-sponsor.svg)][sponsor] [![Gitter](docs/images/badge-gitter.svg)][gitter]
 
      â¨&#xFE0F; This README is a stub. Please see the HTML documentation:
                       marzer.github.io/soagenâ¨&#xFE0F;
 
 
 [gitter]: https://gitter.im/marzer/community [sponsor]: https://github.com/
-sponsors/marzer # Changelog ## v0.1.1 - Minor refactors. ## v0.1.0 - First
-public release ð&#xFE0F;
+sponsors/marzer # Changelog ## v0.1.2 - Minor refactors. ## v0.1.1 - Minor
+refactors. ## v0.1.0 - First public release ð&#xFE0F;
```

### Comparing `soagen-0.1.1/src/soagen.egg-info/SOURCES.txt` & `soagen-0.1.2/src/soagen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

