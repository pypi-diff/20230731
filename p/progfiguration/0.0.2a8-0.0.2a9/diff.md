# Comparing `tmp/progfiguration-0.0.2a8.tar.gz` & `tmp/progfiguration-0.0.2a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progfiguration-0.0.2a8.tar", last modified: Mon Jul 31 00:58:26 2023, max compression
+gzip compressed data, was "progfiguration-0.0.2a9.tar", last modified: Mon Jul 31 04:57:08 2023, max compression
```

## Comparing `progfiguration-0.0.2a8.tar` & `progfiguration-0.0.2a9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 00:58:26.352096 progfiguration-0.0.2a8/
--rw-------   0 mrled      (501) staff       (20)     1074 2023-07-24 04:31:40.000000 progfiguration-0.0.2a8/LICENSE
--rw-------   0 mrled      (501) staff       (20)     3109 2023-07-31 00:58:26.351352 progfiguration-0.0.2a8/PKG-INFO
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 00:58:26.325728 progfiguration-0.0.2a8/progfiguration/
--rw-------   0 mrled      (501) staff       (20)      518 2023-07-23 23:23:06.000000 progfiguration-0.0.2a8/progfiguration/__init__.py
--rw-------   0 mrled      (501) staff       (20)     3635 2023-07-23 21:17:36.000000 progfiguration-0.0.2a8/progfiguration/age.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 00:58:26.328272 progfiguration-0.0.2a8/progfiguration/builddata/
--rw-r--r--   0 mrled      (501) staff       (20)      253 2023-07-22 05:43:26.000000 progfiguration-0.0.2a8/progfiguration/builddata/__init__.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 00:58:26.331766 progfiguration-0.0.2a8/progfiguration/cli/
--rw-------   0 mrled      (501) staff       (20)       41 2023-07-23 22:36:36.000000 progfiguration-0.0.2a8/progfiguration/cli/__init__.py
--rw-------   0 mrled      (501) staff       (20)     6909 2023-07-29 02:11:37.000000 progfiguration-0.0.2a8/progfiguration/cli/progfiguration_core_cmd.py
--rw-r--r--   0 mrled      (501) staff       (20)    21515 2023-07-31 00:57:31.000000 progfiguration-0.0.2a8/progfiguration/cli/progfiguration_site_cmd.py
--rw-r--r--   0 mrled      (501) staff       (20)     5863 2023-07-23 23:10:02.000000 progfiguration-0.0.2a8/progfiguration/cli/util.py
--rw-------   0 mrled      (501) staff       (20)     6669 2023-07-29 04:31:32.000000 progfiguration-0.0.2a8/progfiguration/cmd.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 00:58:26.335219 progfiguration-0.0.2a8/progfiguration/inventory/
--rw-------   0 mrled      (501) staff       (20)    17726 2023-07-29 02:57:14.000000 progfiguration-0.0.2a8/progfiguration/inventory/__init__.py
--rw-------   0 mrled      (501) staff       (20)      874 2023-07-22 04:24:12.000000 progfiguration-0.0.2a8/progfiguration/inventory/nodes.py
--rw-------   0 mrled      (501) staff       (20)     4613 2023-07-23 23:21:39.000000 progfiguration-0.0.2a8/progfiguration/inventory/roles.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 00:58:26.339174 progfiguration-0.0.2a8/progfiguration/localhost/
--rw-------   0 mrled      (501) staff       (20)    11082 2023-07-23 23:21:13.000000 progfiguration-0.0.2a8/progfiguration/localhost/__init__.py
--rw-------   0 mrled      (501) staff       (20)     1184 2023-07-22 04:24:17.000000 progfiguration-0.0.2a8/progfiguration/localhost/authorized_keys.py
--rw-------   0 mrled      (501) staff       (20)     6056 2023-07-22 04:24:20.000000 progfiguration-0.0.2a8/progfiguration/localhost/disks.py
--rw-------   0 mrled      (501) staff       (20)     3044 2023-07-22 04:24:22.000000 progfiguration-0.0.2a8/progfiguration/localhost/localusers.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 00:58:26.343225 progfiguration-0.0.2a8/progfiguration/progfigbuild/
--rw-r--r--   0 mrled      (501) staff       (20)    17404 2023-07-30 22:42:15.000000 progfiguration-0.0.2a8/progfiguration/progfigbuild/__init__.py
--rw-r--r--   0 mrled      (501) staff       (20)     2505 2023-07-22 05:35:59.000000 progfiguration-0.0.2a8/progfiguration/progfigsite_validator.py
--rw-------   0 mrled      (501) staff       (20)      912 2023-07-22 05:36:48.000000 progfiguration-0.0.2a8/progfiguration/progfigtypes.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 00:58:26.344633 progfiguration-0.0.2a8/progfiguration/remotebrute/
--rw-------   0 mrled      (501) staff       (20)     3117 2023-07-22 04:24:58.000000 progfiguration-0.0.2a8/progfiguration/remotebrute/__init__.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 00:58:26.345642 progfiguration-0.0.2a8/progfiguration/sitewrapper/
--rw-r--r--   0 mrled      (501) staff       (20)     3972 2023-07-22 04:26:29.000000 progfiguration-0.0.2a8/progfiguration/sitewrapper/__init__.py
--rw-------   0 mrled      (501) staff       (20)     1804 2023-07-22 05:39:58.000000 progfiguration-0.0.2a8/progfiguration/ssh.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 00:58:26.346666 progfiguration-0.0.2a8/progfiguration/temple/
--rw-------   0 mrled      (501) staff       (20)      744 2023-06-28 22:11:55.000000 progfiguration-0.0.2a8/progfiguration/temple/__init__.py
--rw-r--r--   0 mrled      (501) staff       (20)     1832 2023-07-29 16:02:29.000000 progfiguration-0.0.2a8/progfiguration/util.py
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 00:58:26.327931 progfiguration-0.0.2a8/progfiguration.egg-info/
--rw-------   0 mrled      (501) staff       (20)     3109 2023-07-31 00:58:26.000000 progfiguration-0.0.2a8/progfiguration.egg-info/PKG-INFO
--rw-------   0 mrled      (501) staff       (20)     1108 2023-07-31 00:58:26.000000 progfiguration-0.0.2a8/progfiguration.egg-info/SOURCES.txt
--rw-------   0 mrled      (501) staff       (20)        1 2023-07-31 00:58:26.000000 progfiguration-0.0.2a8/progfiguration.egg-info/dependency_links.txt
--rw-------   0 mrled      (501) staff       (20)       83 2023-07-31 00:58:26.000000 progfiguration-0.0.2a8/progfiguration.egg-info/entry_points.txt
--rw-------   0 mrled      (501) staff       (20)      184 2023-07-31 00:58:26.000000 progfiguration-0.0.2a8/progfiguration.egg-info/requires.txt
--rw-------   0 mrled      (501) staff       (20)       15 2023-07-31 00:58:26.000000 progfiguration-0.0.2a8/progfiguration.egg-info/top_level.txt
--rw-------   0 mrled      (501) staff       (20)     1068 2023-07-31 00:58:05.000000 progfiguration-0.0.2a8/pyproject.toml
--rw-------   0 mrled      (501) staff       (20)     2718 2023-07-29 02:39:31.000000 progfiguration-0.0.2a8/readme.md
--rw-------   0 mrled      (501) staff       (20)       38 2023-07-31 00:58:26.352286 progfiguration-0.0.2a8/setup.cfg
-drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 00:58:26.350068 progfiguration-0.0.2a8/tests/
--rw-------   0 mrled      (501) staff       (20)     1293 2023-07-22 04:15:43.000000 progfiguration-0.0.2a8/tests/test_cmd.py
--rw-------   0 mrled      (501) staff       (20)     1778 2023-07-22 04:38:21.000000 progfiguration-0.0.2a8/tests/test_packaging.py
--rw-------   0 mrled      (501) staff       (20)     2321 2023-07-19 14:30:38.000000 progfiguration-0.0.2a8/tests/test_site.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 04:57:08.919584 progfiguration-0.0.2a9/
+-rw-------   0 mrled      (501) staff       (20)     1074 2023-07-31 02:46:41.000000 progfiguration-0.0.2a9/LICENSE
+-rw-------   0 mrled      (501) staff       (20)     3150 2023-07-31 04:57:08.919072 progfiguration-0.0.2a9/PKG-INFO
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 04:57:08.897283 progfiguration-0.0.2a9/progfiguration/
+-rw-------   0 mrled      (501) staff       (20)      518 2023-07-31 02:46:41.000000 progfiguration-0.0.2a9/progfiguration/__init__.py
+-rw-------   0 mrled      (501) staff       (20)     3635 2023-07-31 02:46:41.000000 progfiguration-0.0.2a9/progfiguration/age.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 04:57:08.903192 progfiguration-0.0.2a9/progfiguration/builddata/
+-rw-------   0 mrled      (501) staff       (20)      253 2023-07-31 02:46:41.000000 progfiguration-0.0.2a9/progfiguration/builddata/__init__.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 04:57:08.906772 progfiguration-0.0.2a9/progfiguration/cli/
+-rw-------   0 mrled      (501) staff       (20)       41 2023-07-31 02:46:41.000000 progfiguration-0.0.2a9/progfiguration/cli/__init__.py
+-rw-------   0 mrled      (501) staff       (20)     6412 2023-07-31 04:41:37.000000 progfiguration-0.0.2a9/progfiguration/cli/progfiguration_core_cmd.py
+-rw-------   0 mrled      (501) staff       (20)    21213 2023-07-31 04:43:20.000000 progfiguration-0.0.2a9/progfiguration/cli/progfiguration_site_cmd.py
+-rw-------   0 mrled      (501) staff       (20)     4025 2023-07-31 04:43:28.000000 progfiguration-0.0.2a9/progfiguration/cli/util.py
+-rw-------   0 mrled      (501) staff       (20)     6669 2023-07-31 02:46:41.000000 progfiguration-0.0.2a9/progfiguration/cmd.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 04:57:08.909395 progfiguration-0.0.2a9/progfiguration/inventory/
+-rw-------   0 mrled      (501) staff       (20)    17726 2023-07-31 02:46:41.000000 progfiguration-0.0.2a9/progfiguration/inventory/__init__.py
+-rw-------   0 mrled      (501) staff       (20)      874 2023-07-31 02:46:41.000000 progfiguration-0.0.2a9/progfiguration/inventory/nodes.py
+-rw-------   0 mrled      (501) staff       (20)     4613 2023-07-31 02:46:41.000000 progfiguration-0.0.2a9/progfiguration/inventory/roles.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 04:57:08.913209 progfiguration-0.0.2a9/progfiguration/localhost/
+-rw-------   0 mrled      (501) staff       (20)    11082 2023-07-31 02:46:41.000000 progfiguration-0.0.2a9/progfiguration/localhost/__init__.py
+-rw-------   0 mrled      (501) staff       (20)     1184 2023-07-31 02:46:41.000000 progfiguration-0.0.2a9/progfiguration/localhost/authorized_keys.py
+-rw-------   0 mrled      (501) staff       (20)     6056 2023-07-31 02:46:41.000000 progfiguration-0.0.2a9/progfiguration/localhost/disks.py
+-rw-------   0 mrled      (501) staff       (20)     3044 2023-07-31 02:46:41.000000 progfiguration-0.0.2a9/progfiguration/localhost/localusers.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 04:57:08.914002 progfiguration-0.0.2a9/progfiguration/progfigbuild/
+-rw-------   0 mrled      (501) staff       (20)    17996 2023-07-31 02:58:33.000000 progfiguration-0.0.2a9/progfiguration/progfigbuild/__init__.py
+-rw-------   0 mrled      (501) staff       (20)     2505 2023-07-31 02:46:41.000000 progfiguration-0.0.2a9/progfiguration/progfigsite_validator.py
+-rw-------   0 mrled      (501) staff       (20)      912 2023-07-31 02:46:41.000000 progfiguration-0.0.2a9/progfiguration/progfigtypes.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 04:57:08.914765 progfiguration-0.0.2a9/progfiguration/remotebrute/
+-rw-------   0 mrled      (501) staff       (20)     3117 2023-07-31 02:46:41.000000 progfiguration-0.0.2a9/progfiguration/remotebrute/__init__.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 04:57:08.915354 progfiguration-0.0.2a9/progfiguration/sitewrapper/
+-rw-------   0 mrled      (501) staff       (20)     3972 2023-07-31 02:46:41.000000 progfiguration-0.0.2a9/progfiguration/sitewrapper/__init__.py
+-rw-------   0 mrled      (501) staff       (20)     1804 2023-07-31 02:46:41.000000 progfiguration-0.0.2a9/progfiguration/ssh.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 04:57:08.915995 progfiguration-0.0.2a9/progfiguration/temple/
+-rw-------   0 mrled      (501) staff       (20)      744 2023-07-31 02:46:41.000000 progfiguration-0.0.2a9/progfiguration/temple/__init__.py
+-rw-------   0 mrled      (501) staff       (20)     1832 2023-07-31 02:46:41.000000 progfiguration-0.0.2a9/progfiguration/util.py
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 04:57:08.902041 progfiguration-0.0.2a9/progfiguration.egg-info/
+-rw-------   0 mrled      (501) staff       (20)     3150 2023-07-31 04:57:08.000000 progfiguration-0.0.2a9/progfiguration.egg-info/PKG-INFO
+-rw-------   0 mrled      (501) staff       (20)     1108 2023-07-31 04:57:08.000000 progfiguration-0.0.2a9/progfiguration.egg-info/SOURCES.txt
+-rw-------   0 mrled      (501) staff       (20)        1 2023-07-31 04:57:08.000000 progfiguration-0.0.2a9/progfiguration.egg-info/dependency_links.txt
+-rw-------   0 mrled      (501) staff       (20)       83 2023-07-31 04:57:08.000000 progfiguration-0.0.2a9/progfiguration.egg-info/entry_points.txt
+-rw-------   0 mrled      (501) staff       (20)      172 2023-07-31 04:57:08.000000 progfiguration-0.0.2a9/progfiguration.egg-info/requires.txt
+-rw-------   0 mrled      (501) staff       (20)       15 2023-07-31 04:57:08.000000 progfiguration-0.0.2a9/progfiguration.egg-info/top_level.txt
+-rw-------   0 mrled      (501) staff       (20)     1015 2023-07-31 04:56:11.000000 progfiguration-0.0.2a9/pyproject.toml
+-rw-------   0 mrled      (501) staff       (20)     2759 2023-07-31 04:55:46.000000 progfiguration-0.0.2a9/readme.md
+-rw-------   0 mrled      (501) staff       (20)       38 2023-07-31 04:57:08.919763 progfiguration-0.0.2a9/setup.cfg
+drwx------   0 mrled      (501) staff       (20)        0 2023-07-31 04:57:08.918108 progfiguration-0.0.2a9/tests/
+-rw-------   0 mrled      (501) staff       (20)     1293 2023-07-31 02:46:41.000000 progfiguration-0.0.2a9/tests/test_cmd.py
+-rw-------   0 mrled      (501) staff       (20)     1778 2023-07-31 02:46:41.000000 progfiguration-0.0.2a9/tests/test_packaging.py
+-rw-------   0 mrled      (501) staff       (20)     2321 2023-07-31 02:46:41.000000 progfiguration-0.0.2a9/tests/test_site.py
```

### Comparing `progfiguration-0.0.2a8/LICENSE` & `progfiguration-0.0.2a9/LICENSE`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a8/PKG-INFO` & `progfiguration-0.0.2a9/readme.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: progfiguration
-Version: 0.0.2a8
-Summary: PROGramatic conFIGURATION for your infrastructure
-Author-email: Micah R Ledbetter <me@micahrl.com>
-License: MIT
-Project-URL: Homepage, https://github.com/mrled/progfiguration
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: development
-Provides-Extra: ghpages-builder
-License-File: LICENSE
-
 # progfiguration
 
 PROGrammatic conFIGURATION.
 I'm tired of writing YAML when what I want to write is Python.
 
 ## Building and publishing
 
@@ -66,15 +53,15 @@
 progfigsite --help
 ```
 
 ## Making a release
 
 1.  Check out the `master` branch.
     Make sure your checkout is clean, with all changes committed to git and pushed to Github
-2.  Set the version in `pyproject.toml`.
+2.  Set the version in `pyproject.toml` and update `docs/appendix/changelog.rst`.
     Don't commit the change yet.
     We'll read this file to determine the version to tag in git and push to PyPI.
     *   This will require Python 3.11 because we parse the TOML file directly with `tomllib`.
     *   We can't use `progfiguration version` for this because it will return the version as it was at install time.
 3.  Run the following:
 
 ```sh
```

### Comparing `progfiguration-0.0.2a8/progfiguration/__init__.py` & `progfiguration-0.0.2a9/progfiguration/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a8/progfiguration/age.py` & `progfiguration-0.0.2a9/progfiguration/age.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a8/progfiguration/cli/progfiguration_core_cmd.py` & `progfiguration-0.0.2a9/progfiguration/cli/progfiguration_core_cmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import pathlib
 import sys
 
 import progfiguration
 from progfiguration import progfigbuild
 from progfiguration.cli.util import (
     configure_logging,
-    get_command_help,
     idb_excepthook,
     progfiguration_error_handler,
     progfiguration_log_levels,
 )
 from progfiguration.progfigsite_validator import validate
 from progfiguration.util import import_module_from_filepath
 
@@ -163,26 +162,7 @@
     else:
         parser.error(f"Unknown action {parsed.action}")
 
 
 def main():
     """The main entry point for the progfiguration command-line interface"""
     progfiguration_error_handler(_main_implementation, *sys.argv)
-
-
-__doc__ = f"""
-The command-line interface to progfiguration core.
-
-This command is installed with the progfiguration package.
-When packaging a progfigsite in a pyz, it is not available.
-
-This command can perform general progfiguration related tasks that don't need a site,
-as well as tasks that validate or build site packages.
-
-## Command line help
-
-The program's command-line help is reproduced here:
-
-```text
-{get_command_help("progfiguration", _make_parser())}
-```
-"""
```

### Comparing `progfiguration-0.0.2a8/progfiguration/cli/progfiguration_site_cmd.py` & `progfiguration-0.0.2a9/progfiguration/cli/progfiguration_site_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,32 @@
 from typing import List, Optional
 
 import progfiguration
 from progfiguration import logger, progfigbuild, remotebrute, sitewrapper
 from progfiguration.cli.util import (
     CommaSeparatedStrList,
     configure_logging,
-    get_command_help,
     idb_excepthook,
     progfiguration_error_handler,
     progfiguration_log_levels,
     syslog_excepthook,
 )
 from progfiguration.inventory import Inventory
 from progfiguration.progfigsite_validator import validate
 
 
 def _action_version_core():
     """Retrieve the version of progfiguration core"""
 
-    coreversion = importlib.metadata.version("progfiguration")
+    try:
+        coreversion = importlib.metadata.version("progfiguration")
+    except importlib.metadata.PackageNotFoundError:
+        # This happens if progfiguration was vendored
+        # TODO: Handle vendored progfiguration version more gracefully
+        coreversion = "vendored"
     result = [
         f"progfiguration core:",
         f"    path: {pathlib.Path(progfiguration.__file__).parent}",
         f"    version: {coreversion}",
     ]
     print("\n".join(result))
 
@@ -550,28 +554,7 @@
     TODO: document how the modpath thing works
     """
     progfiguration.progfigsite_module_path = progfigsite_modpath
 
     # mypy flags this for no reason and I can't figure out why, YOLO
     # > Argument 2 to "progfiguration_error_handler" has incompatible type "*list[str]"; expected "list[str]"  [arg-type]mypy(error)
     progfiguration_error_handler(_main_implementation, *sys.argv)  # type: ignore
-
-
-__doc__ = f"""
-The command-line interface for a progfigsite.
-
-This command is installed with a progfigsite package.
-When packaging a progfigsite in a pyz,
-running the pyz will run this command.
-
-This command can interact with site nodes,
-encrypt and decrypt secrets (if an appropriate private key is available),
-and apply a node's roles to the local machine.
-
-## Command line help
-
-The program's command-line help is reproduced here:
-
-```text
-{get_command_help("progfigsite", _make_parser())}
-```
-"""
```

### Comparing `progfiguration-0.0.2a8/progfiguration/cmd.py` & `progfiguration-0.0.2a9/progfiguration/cmd.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a8/progfiguration/inventory/__init__.py` & `progfiguration-0.0.2a9/progfiguration/inventory/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a8/progfiguration/inventory/nodes.py` & `progfiguration-0.0.2a9/progfiguration/inventory/nodes.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a8/progfiguration/inventory/roles.py` & `progfiguration-0.0.2a9/progfiguration/inventory/roles.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a8/progfiguration/localhost/__init__.py` & `progfiguration-0.0.2a9/progfiguration/localhost/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a8/progfiguration/localhost/authorized_keys.py` & `progfiguration-0.0.2a9/progfiguration/localhost/authorized_keys.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a8/progfiguration/localhost/disks.py` & `progfiguration-0.0.2a9/progfiguration/localhost/disks.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a8/progfiguration/localhost/localusers.py` & `progfiguration-0.0.2a9/progfiguration/localhost/localusers.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a8/progfiguration/progfigbuild/__init__.py` & `progfiguration-0.0.2a9/progfiguration/progfigbuild/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,18 +85,27 @@
 
     if progfiguration_package_path is None:
         progfiguration_package_path = pathlib.Path(progfiguration.__file__).parent
 
     if build_date is None:
         build_date = datetime.utcnow()
 
+    # We need to use the same module path that the progfigsite uses.
+    # Meaning, if the progfigsite is a module name "example_site",
+    # we need to add it to a directory of the same name in the zipfile.
+    # This is because the site will have "from example_site import ..." statements.
+    #
+    # TODO: Not sure what to do if the progfigsite is a dotted package name like "example.site".
+    # That is not a common use case, but might happen because of the --progfigsite-python-path option.
+    site_zip_directory = progfiguration.progfigsite_module_path
+
     main_py = textwrap.dedent(
-        r"""
+        f"""
         from progfiguration.cli import progfiguration_site_cmd
-        progfiguration_site_cmd.main("progfigsite")
+        progfiguration_site_cmd.main("{site_zip_directory}")
         """
     )
 
     def shouldignore(path: pathlib.Path) -> bool:
         """Return True if the path should be excluded from the zipapp file"""
         exacts = [
             "__pycache__",
@@ -127,25 +136,25 @@
             for child in progfigsite_filesystem_path.rglob("*"):
                 if shouldignore(child):
                     continue
                 child_relname = child.relative_to(progfigsite_filesystem_path)
                 # Place the progfigsite package inside a subdirectory called 'progfigsite'.
                 # This ignores the actual name of the package,
                 # and allows progfiguration to find it when run from the zipfile.
-                z.write(child, "progfigsite/" + child_relname.as_posix())
+                z.write(child, site_zip_directory + "/" + child_relname.as_posix())
 
             # Copy the progfiguration package into the zipfile
             for child in progfiguration_package_path.rglob("*"):
                 if shouldignore(child):
                     continue
                 child_relname = child.relative_to(progfiguration_package_path)
                 z.write(child, "progfiguration/" + child_relname.as_posix())
 
             # Inject build date file
-            z.writestr("progfigsite/builddata/version.py", builddata_version_py.encode("utf-8"))
+            z.writestr(site_zip_directory + "/builddata/version.py", builddata_version_py.encode("utf-8"))
 
             # Add the __main__.py file to the zipfile root, which is required for zipapps
             z.writestr("__main__.py", main_py.encode("utf-8"))
 
     # Make the zipapp executable
     package_out_path.chmod(package_out_path.stat().st_mode | stat.S_IEXEC)
```

### Comparing `progfiguration-0.0.2a8/progfiguration/progfigsite_validator.py` & `progfiguration-0.0.2a9/progfiguration/progfigsite_validator.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a8/progfiguration/progfigtypes.py` & `progfiguration-0.0.2a9/progfiguration/progfigtypes.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a8/progfiguration/remotebrute/__init__.py` & `progfiguration-0.0.2a9/progfiguration/remotebrute/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a8/progfiguration/sitewrapper/__init__.py` & `progfiguration-0.0.2a9/progfiguration/sitewrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a8/progfiguration/ssh.py` & `progfiguration-0.0.2a9/progfiguration/ssh.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a8/progfiguration/temple/__init__.py` & `progfiguration-0.0.2a9/progfiguration/temple/__init__.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a8/progfiguration/util.py` & `progfiguration-0.0.2a9/progfiguration/util.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a8/progfiguration.egg-info/PKG-INFO` & `progfiguration-0.0.2a9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progfiguration
-Version: 0.0.2a8
+Version: 0.0.2a9
 Summary: PROGramatic conFIGURATION for your infrastructure
 Author-email: Micah R Ledbetter <me@micahrl.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mrled/progfiguration
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: development
@@ -66,15 +66,15 @@
 progfigsite --help
 ```
 
 ## Making a release
 
 1.  Check out the `master` branch.
     Make sure your checkout is clean, with all changes committed to git and pushed to Github
-2.  Set the version in `pyproject.toml`.
+2.  Set the version in `pyproject.toml` and update `docs/appendix/changelog.rst`.
     Don't commit the change yet.
     We'll read this file to determine the version to tag in git and push to PyPI.
     *   This will require Python 3.11 because we parse the TOML file directly with `tomllib`.
     *   We can't use `progfiguration version` for this because it will return the version as it was at install time.
 3.  Run the following:
 
 ```sh
```

### Comparing `progfiguration-0.0.2a8/progfiguration.egg-info/SOURCES.txt` & `progfiguration-0.0.2a9/progfiguration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a8/pyproject.toml` & `progfiguration-0.0.2a9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "progfiguration"
-version = "0.0.2a8"
+version = "0.0.2a9"
 description = "PROGramatic conFIGURATION for your infrastructure"
 license = { text = "MIT" }
 readme = "readme.md"
 requires-python = ">=3.10"
 
 [[project.authors]]
 name = "Micah R Ledbetter"
@@ -21,15 +21,14 @@
 
 # Used for local development
 development = [
     "black",
     "build",
     "furo",             # Sphinx theme
     "mypy",
-    "myst_parser",      # markdown support in Sphinx
     "sphinx",
     "sphinx-argparse",
     "sphinx-autoapi",
     "sphinx-autobuild",
     "twine",
 ]
```

### Comparing `progfiguration-0.0.2a8/readme.md` & `progfiguration-0.0.2a9/progfiguration.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: progfiguration
+Version: 0.0.2a9
+Summary: PROGramatic conFIGURATION for your infrastructure
+Author-email: Micah R Ledbetter <me@micahrl.com>
+License: MIT
+Project-URL: Homepage, https://github.com/mrled/progfiguration
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: development
+Provides-Extra: ghpages-builder
+License-File: LICENSE
+
 # progfiguration
 
 PROGrammatic conFIGURATION.
 I'm tired of writing YAML when what I want to write is Python.
 
 ## Building and publishing
 
@@ -53,15 +66,15 @@
 progfigsite --help
 ```
 
 ## Making a release
 
 1.  Check out the `master` branch.
     Make sure your checkout is clean, with all changes committed to git and pushed to Github
-2.  Set the version in `pyproject.toml`.
+2.  Set the version in `pyproject.toml` and update `docs/appendix/changelog.rst`.
     Don't commit the change yet.
     We'll read this file to determine the version to tag in git and push to PyPI.
     *   This will require Python 3.11 because we parse the TOML file directly with `tomllib`.
     *   We can't use `progfiguration version` for this because it will return the version as it was at install time.
 3.  Run the following:
 
 ```sh
```

### Comparing `progfiguration-0.0.2a8/tests/test_cmd.py` & `progfiguration-0.0.2a9/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a8/tests/test_packaging.py` & `progfiguration-0.0.2a9/tests/test_packaging.py`

 * *Files identical despite different names*

### Comparing `progfiguration-0.0.2a8/tests/test_site.py` & `progfiguration-0.0.2a9/tests/test_site.py`

 * *Files identical despite different names*

