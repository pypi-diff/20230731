# Comparing `tmp/changelog-parser-0.0.1.tar.gz` & `tmp/changelog-parser-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "changelog-parser-0.0.1.tar", last modified: Fri Jul 28 20:04:49 2023, max compression
+gzip compressed data, was "changelog-parser-0.0.2.tar", last modified: Mon Jul 31 16:42:35 2023, max compression
```

## Comparing `changelog-parser-0.0.1.tar` & `changelog-parser-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:04:49.005756 changelog-parser-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:04:49.001756 changelog-parser-0.0.1/.github/
--rwxr-xr-x   0 runner    (1001) docker     (123)       16 2023-07-28 20:04:36.000000 changelog-parser-0.0.1/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:04:49.001756 changelog-parser-0.0.1/.github/workflows/
--rwxr-xr-x   0 runner    (1001) docker     (123)      425 2023-07-28 20:04:36.000000 changelog-parser-0.0.1/.github/workflows/deploy.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      272 2023-07-28 20:04:36.000000 changelog-parser-0.0.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-28 20:04:36.000000 changelog-parser-0.0.1/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      446 2023-07-28 20:04:36.000000 changelog-parser-0.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-28 20:04:36.000000 changelog-parser-0.0.1/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      533 2023-07-28 20:04:36.000000 changelog-parser-0.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-28 20:04:49.005756 changelog-parser-0.0.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1909 2023-07-28 20:04:36.000000 changelog-parser-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:04:49.001756 changelog-parser-0.0.1/changelog_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-28 20:04:48.000000 changelog-parser-0.0.1/changelog_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-28 20:04:48.000000 changelog-parser-0.0.1/changelog_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:04:48.000000 changelog-parser-0.0.1/changelog_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 20:04:48.000000 changelog-parser-0.0.1/changelog_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 20:04:48.000000 changelog-parser-0.0.1/changelog_parser.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1291 2023-07-28 20:04:36.000000 changelog-parser-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:04:49.005756 changelog-parser-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:04:49.005756 changelog-parser-0.0.1/src/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7585 2023-07-28 20:04:36.000000 changelog-parser-0.0.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:04:49.005756 changelog-parser-0.0.1/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-07-28 20:04:36.000000 changelog-parser-0.0.1/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:04:49.001756 changelog-parser-0.0.1/test/projects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:04:49.005756 changelog-parser-0.0.1/test/projects/example/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8039 2023-07-28 20:04:36.000000 changelog-parser-0.0.1/test/projects/example/CHANGELOG.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     2789 2023-07-28 20:04:36.000000 changelog-parser-0.0.1/test/test_load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:42:35.566761 changelog-parser-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:42:35.566761 changelog-parser-0.0.2/.github/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       16 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:42:35.566761 changelog-parser-0.0.2/.github/workflows/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      425 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/.github/workflows/deploy.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      272 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      552 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      533 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-31 16:42:35.566761 changelog-parser-0.0.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1909 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:42:35.566761 changelog-parser-0.0.2/changelog_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-07-31 16:42:35.000000 changelog-parser-0.0.2/changelog_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-31 16:42:35.000000 changelog-parser-0.0.2/changelog_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 16:42:35.000000 changelog-parser-0.0.2/changelog_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-31 16:42:35.000000 changelog-parser-0.0.2/changelog_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-31 16:42:35.000000 changelog-parser-0.0.2/changelog_parser.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1305 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 16:42:35.566761 changelog-parser-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:42:35.566761 changelog-parser-0.0.2/src/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7673 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:42:35.566761 changelog-parser-0.0.2/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:42:35.566761 changelog-parser-0.0.2/test/projects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:42:35.566761 changelog-parser-0.0.2/test/projects/example/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8039 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/test/projects/example/CHANGELOG.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2797 2023-07-31 16:42:26.000000 changelog-parser-0.0.2/test/test_load.py
```

### Comparing `changelog-parser-0.0.1/.gitignore` & `changelog-parser-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `changelog-parser-0.0.1/LICENSE` & `changelog-parser-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `changelog-parser-0.0.1/Makefile` & `changelog-parser-0.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `changelog-parser-0.0.1/PKG-INFO` & `changelog-parser-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changelog-parser
-Version: 0.0.1
+Version: 0.0.2
 Summary: Parses changelog files
 Author-email: Jason Stiefel <Jason.R.Stiefel@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 JasonStiefel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `changelog-parser-0.0.1/README.md` & `changelog-parser-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `changelog-parser-0.0.1/changelog_parser.egg-info/PKG-INFO` & `changelog-parser-0.0.2/changelog_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changelog-parser
-Version: 0.0.1
+Version: 0.0.2
 Summary: Parses changelog files
 Author-email: Jason Stiefel <Jason.R.Stiefel@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 JasonStiefel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `changelog-parser-0.0.1/pyproject.toml` & `changelog-parser-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "changelog-parser"
-version = "0.0.1"
 description = "Parses changelog files"
 readme = "README.md"
 requires-python = ">= 3.8"
 license.file = "LICENSE"
 authors = [
   { name = "Jason Stiefel", email = "Jason.R.Stiefel@gmail.com" }
 ]
@@ -22,29 +21,28 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 urls.homepage = "https://github.com/JasonStiefel/changelog-parser"
 urls.changelog = "https://github.com/JasonStiefel/changelog-parser/blob/main/CHANGELOG.md"
+dynamic = [ "version" ]
 
 dependencies = [
   "semver"
 ]
 
+[tool.setuptools.dynamic]
+version = { attr = "changelog.__version__" }
+
 [project.optional-dependencies]
 test = [
   "pytest",
   "pytest-xdist"
 ]
 
 [tool.pytest.ini_options]
 log_cli_level = "info"
 testpaths = [ "test" ]
 
 [tool.setuptools.package-dir]
 changelog = "src"
-
-[tool.setuptools.package-data]
-profile_service = [
-  "*.ini"
-]
```

### Comparing `changelog-parser-0.0.1/src/__init__.py` & `changelog-parser-0.0.2/src/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 # SPDX-License-Identifier: MIT
 
-__version__ = '0.0.0'
+__version__ = '0.0.2'
 
 import re
 from datetime import date
 from semver import Version
 from typing import ( Optional, Any )
 from io import ( IOBase, StringIO )
 
 class ChangelogParsingError(Exception):
     @property
-    def line_no( self )-> Optional[ int ]:
+    def line_number( self )-> Optional[ int ]:
         if ( match := re.search( r' \(at line (\d+)(?:, column \d+)?\)$', str( self ) ) ):
             return int( match.group( 1 ) )
 
     @property
-    def column_no( self )-> Optional[ int ]:
+    def column_number( self )-> Optional[ int ]:
         if ( match := re.search( r' \(at (?:line \d+, )?column (\d+)\)$', str( self ) ) ):
             return int( match.group( 1 ) )
 
-    def __init__( self, msg: str, line_no: Optional[ int ] = None, column_no: Optional[ int ] = None ):
+    def __init__( self, msg: str, line_number: Optional[ int ] = None, column_number: Optional[ int ] = None ):
         specifications = (
-            *( ( f'line { line_no }', ) if isinstance( line_no, int ) else () ),
-            *( ( f'column { column_no }', ) if isinstance( column_no, int ) else () )
+            *( ( f'line { line_number }', ) if isinstance( line_number, int ) else () ),
+            *( ( f'column { column_number }', ) if isinstance( column_number, int ) else () )
         )
         super().__init__( msg + ( f' (at { ", ".join( specifications ) })' if specifications else '' ) )
 
 def load( fp: IOBase, encoding: str = 'utf-8' )-> dict[ str, Any ]:
     line_no, changes, section, in_compare_urls = 0, [], None, False
 
     while ( line := fp.readline() ):
         line_no += 1
         if isinstance( line, bytes ):
             try:
                 line = line.decode( encoding )
             except Exception as e:
                 raise ChangelogParsingError(
                     msg = f'Unable to decode line using encoding, "{ encoding }"; { e }',
-                    line_no = line_no
+                    line_number = line_no
                 )
         if isinstance( line, str ):
             line = line.removesuffix( '\n' )
         else:
             raise ChangelogParsingError(
                 f'Parameter\'s "readline" function call returned unreadable type, "{ type( line ).__name__ }"'
             )
@@ -53,16 +53,16 @@
                 section = None
 
             changes.append( { "date": None,  } )
 
             if line.rstrip() != line:
                 raise ChangelogParsingError(
                     msg = "Extra space(s) at end of line",
-                    line_no = line_no,
-                    column_no = len( line.rstrip() ) + 1
+                    line_number = line_no,
+                    column_number = len( line.rstrip() ) + 1
                 )
             if line.endswith( " [YANKED]" ):
                 changes[ -1 ][ "yanked" ] = True
                 line = line.removesuffix( " [YANKED]" )
             else:
                 changes[ -1 ][ "yanked" ] = False
 
@@ -73,33 +73,33 @@
                 raise ChangelogParsingError( "Extra space(s) before date", line_no, len( line + sep ) + 1 )
             if sep:
                 try:
                     changes[ -1 ][ "date" ] = date.fromisoformat( change_date )
                 except Exception as e:
                     raise ChangelogParsingError(
                         msg = f'Unable to parse changelog entry date, "{ change_date }"; { e }',
-                        line_no = line_no,
-                        column_no = len( line + sep ) + 1
+                        line_number = line_no,
+                        column_number = len( line + sep ) + 1
                     )
 
             if line.rstrip() != line:
                 raise ChangelogParsingError(
                     msg = "Extra space(s) after version",
-                    line_no = line_no,
-                    column_no = len( line.rstrip() ) + 1
+                    line_number = line_no,
+                    column_number = len( line.rstrip() ) + 1
                 )
             line = line.removeprefix( "## " )
             if line.lstrip() != line:
                 raise ChangelogParsingError( "Extra space(s) before version", line_no, 4 )
 
             if not line.startswith( "[" ) or not line.endswith( "]" ):
                 raise ChangelogParsingError(
                     msg = 'Version must be enclosed with square brackets',
-                    line_no = line_no,
-                    column_no = 4 if not line.startswith( "[" ) else 4 + len( line )
+                    line_number = line_no,
+                    column_number = 4 if not line.startswith( "[" ) else 4 + len( line )
                 )
             line = line.removeprefix( "[" ).removesuffix( "]" )
             try:
                 changes[ -1 ][ "version" ] = line if line.lower() == "unreleased" else Version.parse( line )
             except Exception as e:
                 raise ChangelogParsingError( f'Failed parsing semver version, "{ line }"; { e }', line_no, 5 )
 
@@ -130,42 +130,42 @@
                 version = match.group( 1 )
             else:
                 try:
                     version = Version.parse( match.group( 1 ) )
                 except Exception as e:
                     raise ChangelogParsingError(
                         msg = f'Failed parsing semver version, "{ match.group( 1 ) }"; { e }',
-                        line_no = line_no,
-                        column_no = 2
+                        line_number = line_no,
+                        column_number = 2
                     )
 
             for change in changes:
                 if isinstance( change[ "version" ], str ) and isinstance( version, str ):
                     if change[ "version" ].lower() == version.lower():
                         break
                 if isinstance( change[ "version" ], Version ) and isinstance( version, Version ):
                     if change[ "version" ] == version:
                         break
             else:
                 raise ChangelogParsingError(
                     msg = f'No corresponding record for compare url with version, "{ match.group( 1 ) }"',
-                    line_no = line_no,
-                    column_no = 2
+                    line_number = line_no,
+                    column_number = 2
                 )
 
             change[ "compare_url" ] = match.group( 2 )
             in_compare_urls = True
 
         elif not line:
             continue
 
         elif in_compare_urls:
             raise ChangelogParsingError(
                 f'After compare URL definitions have started, no other line types are allowed',
-                line_no = line_no
+                line_number = line_no
             )
 
         else:
             raise ChangelogParsingError( f'Unrecognized line pattern, "{ line }"', line_no )
 
     if section is not None and changes[ -1 ][ section ]:
         changes[ -1 ][ section ][ -1 ] = changes[ -1 ][ section ][ -1 ].rstrip()
```

### Comparing `changelog-parser-0.0.1/test/conftest.py` & `changelog-parser-0.0.2/test/conftest.py`

 * *Files identical despite different names*

### Comparing `changelog-parser-0.0.1/test/projects/example/CHANGELOG.md` & `changelog-parser-0.0.2/test/projects/example/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `changelog-parser-0.0.1/test/test_load.py` & `changelog-parser-0.0.2/test/test_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,11 +34,11 @@
     ])
 def test_basic_error_line_patterns( changelog_contents, error_message, msg_line_no, msg_col_no ):
     try:
         changelog.loads( changelog_contents )
     except Exception as e:
         assert isinstance( e, changelog.ChangelogParsingError )
         assert str( e ) == error_message
-        assert e.line_no == msg_line_no
-        assert e.column_no == msg_col_no
+        assert e.line_number == msg_line_no
+        assert e.column_number == msg_col_no
     else:
         pytest.fail( "Loading CHANGELOG did raise an exception" )
```

