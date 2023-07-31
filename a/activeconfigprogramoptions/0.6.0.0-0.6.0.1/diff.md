# Comparing `tmp/activeconfigprogramoptions-0.6.0.0.tar.gz` & `tmp/activeconfigprogramoptions-0.6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activeconfigprogramoptions-0.6.0.0.tar", max compression
+gzip compressed data, was "activeconfigprogramoptions-0.6.0.1.tar", max compression
```

## Comparing `activeconfigprogramoptions-0.6.0.0.tar` & `activeconfigprogramoptions-0.6.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     5024 2023-07-07 01:38:30.253385 activeconfigprogramoptions-0.6.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1732 2023-06-29 23:54:47.460732 activeconfigprogramoptions-0.6.0.0/LICENSE
--rw-r--r--   0        0        0    18936 2023-07-07 01:37:09.253440 activeconfigprogramoptions-0.6.0.0/README.md
--rw-r--r--   0        0        0     2051 2023-07-07 02:11:01.992822 activeconfigprogramoptions-0.6.0.0/pyproject.toml
--rw-r--r--   0        0        0    31908 2023-07-07 01:20:57.833735 activeconfigprogramoptions-0.6.0.0/src/activeconfigprogramoptions/ActiveConfigProgramOptions.py
--rw-r--r--   0        0        0    22156 2023-07-07 01:20:57.833735 activeconfigprogramoptions-0.6.0.0/src/activeconfigprogramoptions/ActiveConfigProgramOptionsCMake.py
--rw-r--r--   0        0        0     2623 2023-07-07 01:20:57.833735 activeconfigprogramoptions-0.6.0.0/src/activeconfigprogramoptions/__init__.py
--rw-r--r--   0        0        0     3289 2023-07-07 01:20:57.833735 activeconfigprogramoptions-0.6.0.0/src/activeconfigprogramoptions/common.py
--rw-r--r--   0        0        0     2427 2023-07-07 01:20:57.833735 activeconfigprogramoptions-0.6.0.0/src/activeconfigprogramoptions/unittests/__init__.py
--rw-r--r--   0        0        0     7322 2023-07-07 01:20:57.833735 activeconfigprogramoptions-0.6.0.0/src/activeconfigprogramoptions/unittests/common.py
--rw-r--r--   0        0        0     6572 2023-07-07 01:20:57.833735 activeconfigprogramoptions-0.6.0.0/src/activeconfigprogramoptions/unittests/files_ini/config_test_activeconfigprogramoptions.ini
--rw-r--r--   0        0        0    22543 2023-07-07 01:20:57.833735 activeconfigprogramoptions-0.6.0.0/src/activeconfigprogramoptions/unittests/test_ActiveConfigProgramOptions.py
--rw-r--r--   0        0        0    32338 2023-07-07 01:20:57.833735 activeconfigprogramoptions-0.6.0.0/src/activeconfigprogramoptions/unittests/test_ActiveConfigProgramOptionsCMake.py
--rw-r--r--   0        0        0     2517 2023-07-07 01:20:57.833735 activeconfigprogramoptions-0.6.0.0/src/activeconfigprogramoptions/version.py
--rw-r--r--   0        0        0    20537 1970-01-01 00:00:00.000000 activeconfigprogramoptions-0.6.0.0/PKG-INFO
+-rw-r--r--   0        0        0     5091 2023-07-31 00:27:36.271484 activeconfigprogramoptions-0.6.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1732 2023-06-29 23:54:47.460732 activeconfigprogramoptions-0.6.0.1/LICENSE
+-rw-r--r--   0        0        0    18936 2023-07-07 01:37:09.253440 activeconfigprogramoptions-0.6.0.1/README.md
+-rw-r--r--   0        0        0     2043 2023-07-31 00:24:40.241514 activeconfigprogramoptions-0.6.0.1/pyproject.toml
+-rw-r--r--   0        0        0    31913 2023-07-31 00:25:34.621504 activeconfigprogramoptions-0.6.0.1/src/activeconfigprogramoptions/ActiveConfigProgramOptions.py
+-rw-r--r--   0        0        0    22147 2023-07-31 00:26:16.551497 activeconfigprogramoptions-0.6.0.1/src/activeconfigprogramoptions/ActiveConfigProgramOptionsCMake.py
+-rw-r--r--   0        0        0     2623 2023-07-07 01:20:57.833735 activeconfigprogramoptions-0.6.0.1/src/activeconfigprogramoptions/__init__.py
+-rw-r--r--   0        0        0     3289 2023-07-07 01:20:57.833735 activeconfigprogramoptions-0.6.0.1/src/activeconfigprogramoptions/common.py
+-rw-r--r--   0        0        0     2427 2023-07-07 01:20:57.833735 activeconfigprogramoptions-0.6.0.1/src/activeconfigprogramoptions/unittests/__init__.py
+-rw-r--r--   0        0        0     7322 2023-07-07 01:20:57.833735 activeconfigprogramoptions-0.6.0.1/src/activeconfigprogramoptions/unittests/common.py
+-rw-r--r--   0        0        0     6572 2023-07-07 01:20:57.833735 activeconfigprogramoptions-0.6.0.1/src/activeconfigprogramoptions/unittests/files_ini/config_test_activeconfigprogramoptions.ini
+-rw-r--r--   0        0        0    22543 2023-07-07 01:20:57.833735 activeconfigprogramoptions-0.6.0.1/src/activeconfigprogramoptions/unittests/test_ActiveConfigProgramOptions.py
+-rw-r--r--   0        0        0    32338 2023-07-07 01:20:57.833735 activeconfigprogramoptions-0.6.0.1/src/activeconfigprogramoptions/unittests/test_ActiveConfigProgramOptionsCMake.py
+-rw-r--r--   0        0        0     2517 2023-07-31 00:25:04.951510 activeconfigprogramoptions-0.6.0.1/src/activeconfigprogramoptions/version.py
+-rw-r--r--   0        0        0    20529 1970-01-01 00:00:00.000000 activeconfigprogramoptions-0.6.0.1/PKG-INFO
```

### Comparing `activeconfigprogramoptions-0.6.0.0/CHANGELOG.md` & `activeconfigprogramoptions-0.6.0.1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,60 +3,64 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 <!--
 ## [X.Y.Z] - YYYY-MM-DD or [Unreleased]
-#### Added
-#### Changed
-#### Deprecated
-#### Removed
-#### Fixed
-#### Security
-#### Internal
-#### Todo (for Unreleased)
+### Added
+### Changed
+### Deprecated
+### Removed
+### Fixed
+### Security
+### Internal
+### Documentation
+### Todo (for Unreleased)
 -->
 
+## [0.6.0.1] 2023-07-31
+### Documentation
+- Minor documentation updates and fixes
 
 
 ## [0.6.0.0] 2023-07-07
-#### Changed
+### Changed
 - Rename package to ActiveConfigProgramOptions
 - Repository updated to use ActiveConfigParser rather than ConfigParserEnhanced.
-#### Deprecated
+### Deprecated
 - Note: Backwards compatibility with SetProgramOptions from github not guaranteed
   because this will use the newer ActiveConfigParser software stack.
 
 
 
 ## [0.5.0.2] 2022-01-07
-#### Changed
+### Changed
 - Documentation updates
 
 
 
 ## [0.5.0.1] 2021-12-30
-#### Changed
+### Changed
 - Documentation updates
 
 
 
 ## [0.5.0] 2021-12-20
-#### Added
+### Added
 - Open Source License approved. Adding 3-Clause BSD license files and
   source headers.
 - github actions files for CI/CD testing will be added to this version
   number once code is posted to https://github.com/sandialabs/SetProgramOptions
 
 
 
 ## [0.4.0] 2021-11-23
-#### Added
-#### Changed
+### Added
+### Changed
 - Changes to `opt-set-cmake-var` behaviour:
   - Trigger a WARNING if `PARENT_SCOPE` and a _TYPE_ is provided since CMake
     requires TYPED vars to be CACHE vars and `PARENT_SCOPE` will force the
     var to be considered a non CACHE var that would store the parameters
     before `PARENT_SCOPE` in the call as _list_ entries. (TRILFRAME-128)
   - Trigger an exception if `PARENT_SCOPE` and `FORCE` are both provided since
     `FORCE` is only valid for CACHE variables but `PARENT_SCOPE` is only valid
@@ -76,59 +80,59 @@
   BASH output if there is an unhandled CMake variable left hanging around.
   Rather than make this an unavoidable error though, ExpandVarsInText now inherits
   from `configparserenhanced.ExceptionControl` and will raise a "MINOR"
   `exception_control_event` (i.e., throws if `exception_control_level` is 4 or greater).
   We also tie this _ecl_ to the _ecl_ of the `SetProgramOptions` class so changing this
   will affect whether or not the exception is raised or if the output returned is an
   empty string.
-#### Deprecated
-#### Removed
-#### Fixed
+### Deprecated
+### Removed
+### Fixed
 - Bash generation handling of the FORCE flag. See TRILFRAME-120 for details.
-#### Security
-#### Internal
+### Security
+### Internal
 - Add test to verify that `opt-remove` also works to remove variables added
   by `opt-set-cmake-var`.
 - Changed `VariableFieldData` so that it won't use `dataclasses` to keep our
   Python compatibilty to 3.6 (`dataclasses` requires 3.7 and higher).
-#### Todo (for Unreleased)
+### Todo (for Unreleased)
 
 
 
 ## [0.3.0] - 2021-06-15
-#### Added
-#### Changed
+### Added
+### Changed
 - Relocated `setprogramoptions` package to `src/`
 - Relocated _examples_ into `examples/` directory.
 - Improved `gitlab-ci.yml` pipeline.
-#### Deprecated
-#### Removed
-#### Fixed
-#### Security
-#### Internal
-#### Todo (for Unreleased)
+### Deprecated
+### Removed
+### Fixed
+### Security
+### Internal
+### Todo (for Unreleased)
 
 
 
 ## [0.2.0] - 2021-06-08
-#### Added
+### Added
 - `common.py` - moved some free-functions to this.
 - Improved *variable* processing. Variables should now be encoded in our pseudo-langauge
   that has a syntax like this: `${VARNAME|VARTYPE}`.
   - `ENV` - is the only 'type' that is known to `SetProgramOptions`
   - `CMAKE` - is known to `SetProgramOptionsCMake`, which denotes a "CMake" variable
     which would be part of the internal state. This mostly makes sense when generating
     CMake Fragments, but we also attempt to track variables that are set when generating
     BASH output and will perform expansions when a prevoulsly set value is known.
   - A `ValueError` will be raised if "BASH" output generation is attempted with a "CMAKE"
     var type still embedded in the .ini file.
-#### Changed
+### Changed
 - _values_ containing spaces in them will have double quotes (`"`) added to them.
-#### Internal
+### Internal
 - Modified `_gen_option_entry` to detect values with spaces in them and add quotes (`"`) to the string.
 
 
 
 ## [0.1.0] - 2021-04-29
-#### Added
+### Added
 - Initial version release. From now on changes should be noted in the
   CHANGELOG.
```

### Comparing `activeconfigprogramoptions-0.6.0.0/LICENSE` & `activeconfigprogramoptions-0.6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `activeconfigprogramoptions-0.6.0.0/README.md` & `activeconfigprogramoptions-0.6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `activeconfigprogramoptions-0.6.0.0/pyproject.toml` & `activeconfigprogramoptions-0.6.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "activeconfigprogramoptions"
 description = "Program options configuration file reader using ActiveConfigParser."
-version = "0.6.0.0"
+version = "0.6.0.1"
 license = "LICENSE"
 readme = "README.md"
 keywords = [
     "Utility",
     "Bash",
     "Configuration",
     "ActiveConfigParser",
     "ConfigParser"
 ]
 authors = [
-    "William McLendon <Semantik-Code@outlook.com>"
+    "William <Semantik-Codeworks@outlook.com>"
 ]
 maintainers = [
-    "William McLendon <Semantik-Code@outlook.com>",
+    "William <Semantik-Codeworks@outlook.com>",
 ]
 homepage      = "https://gitlab.com/semantik-software/code/python/ActiveConfigProgramOptions"
 documentation = "https://semantik-software.gitlab.io/code/python/ActiveConfigProgramOptions"
 repository    = "https://gitlab.com/semantik-software/code/python/ActiveConfigProgramOptions"
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
```

### Comparing `activeconfigprogramoptions-0.6.0.0/src/activeconfigprogramoptions/ActiveConfigProgramOptions.py` & `activeconfigprogramoptions-0.6.0.1/src/activeconfigprogramoptions/ActiveConfigProgramOptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 2. If the ``SUBSTR`` parameter is included, the matching criteria
    is relaxed so that an option is removed from the list if any of
    its parameters *contains* ``Param1`` (i.e., ``Param1`` is a
    *sub string* of any paramter in the option).
 
 
 :Authors:
-    - William C. McLendon III <wcmclen@sandia.gov>
+    - William McLendon <Semantik-Codeworks@outlook.com>
 """
 
 # For type-hinting
 from typing import Dict, Iterable, List, Optional, Set, Tuple, Union
 
 try:                         # pragma: no cover
                              # @final decorator, requires Python 3.8.x
```

### Comparing `activeconfigprogramoptions-0.6.0.0/src/activeconfigprogramoptions/ActiveConfigProgramOptionsCMake.py` & `activeconfigprogramoptions-0.6.0.1/src/activeconfigprogramoptions/ActiveConfigProgramOptionsCMake.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,16 +81,16 @@
 See CMake documentation on the `set() <https://cmake.org/cmake/help/latest/command/set.html>`_
 command for more information on how fragment file entries are generated.
 
 We do not support the *environment variable* variation of ``set()`` at this time.
 
 
 :Authors:
-    - William C. McLendon III <wcmclen@sandia.gov>
-    - Evan Harvey <eharvey@sandia.gov>
+    - William C. McLendon III <Semantik-Codeworks@outlook.com>
+    - Evan Harvey
 """
 from __future__ import print_function
 from enum import Enum
 
 #import inspect
 #from pathlib import Path
 #from textwrap import dedent
```

### Comparing `activeconfigprogramoptions-0.6.0.0/src/activeconfigprogramoptions/__init__.py` & `activeconfigprogramoptions-0.6.0.1/src/activeconfigprogramoptions/__init__.py`

 * *Files identical despite different names*

### Comparing `activeconfigprogramoptions-0.6.0.0/src/activeconfigprogramoptions/common.py` & `activeconfigprogramoptions-0.6.0.1/src/activeconfigprogramoptions/common.py`

 * *Files identical despite different names*

### Comparing `activeconfigprogramoptions-0.6.0.0/src/activeconfigprogramoptions/unittests/__init__.py` & `activeconfigprogramoptions-0.6.0.1/src/activeconfigprogramoptions/unittests/__init__.py`

 * *Files identical despite different names*

### Comparing `activeconfigprogramoptions-0.6.0.0/src/activeconfigprogramoptions/unittests/common.py` & `activeconfigprogramoptions-0.6.0.1/src/activeconfigprogramoptions/unittests/common.py`

 * *Files identical despite different names*

### Comparing `activeconfigprogramoptions-0.6.0.0/src/activeconfigprogramoptions/unittests/files_ini/config_test_activeconfigprogramoptions.ini` & `activeconfigprogramoptions-0.6.0.1/src/activeconfigprogramoptions/unittests/files_ini/config_test_activeconfigprogramoptions.ini`

 * *Files identical despite different names*

### Comparing `activeconfigprogramoptions-0.6.0.0/src/activeconfigprogramoptions/unittests/test_ActiveConfigProgramOptions.py` & `activeconfigprogramoptions-0.6.0.1/src/activeconfigprogramoptions/unittests/test_ActiveConfigProgramOptions.py`

 * *Files identical despite different names*

### Comparing `activeconfigprogramoptions-0.6.0.0/src/activeconfigprogramoptions/unittests/test_ActiveConfigProgramOptionsCMake.py` & `activeconfigprogramoptions-0.6.0.1/src/activeconfigprogramoptions/unittests/test_ActiveConfigProgramOptionsCMake.py`

 * *Files identical despite different names*

### Comparing `activeconfigprogramoptions-0.6.0.0/src/activeconfigprogramoptions/version.py` & `activeconfigprogramoptions-0.6.0.1/src/activeconfigprogramoptions/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #===============================================================================
 
 # Note: When updating this we should also update the
 #       version string in the header docstrings for
 #       ActiveConfigProgramOptions and the pyproject.toml
 #       file.
-__version__ = "0.6.0.0"
+__version__ = "0.6.0.1"
```

### Comparing `activeconfigprogramoptions-0.6.0.0/PKG-INFO` & `activeconfigprogramoptions-0.6.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: activeconfigprogramoptions
-Version: 0.6.0.0
+Version: 0.6.0.1
 Summary: Program options configuration file reader using ActiveConfigParser.
 Home-page: https://gitlab.com/semantik-software/code/python/ActiveConfigProgramOptions
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
 Requires-Python: >=3.6
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
```

