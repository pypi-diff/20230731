# Comparing `tmp/mozregression-5.7.0.dev3.tar.gz` & `tmp/mozregression-5.7.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozregression-5.7.0.dev3.tar", last modified: Tue Jul 25 19:12:48 2023, max compression
+gzip compressed data, was "mozregression-5.7.1.dev0.tar", last modified: Mon Jul 31 14:33:20 2023, max compression
```

## Comparing `mozregression-5.7.0.dev3.tar` & `mozregression-5.7.1.dev0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:48.882218 mozregression-5.7.0.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/.coveralls.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:48.874217 mozregression-5.7.0.dev3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:48.874217 mozregression-5.7.0.dev3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/.github/workflows/compile-requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/.github/workflows/deploy-gui.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/.github/workflows/glean-probe-scraper.yml
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/.github/workflows/run-compile-requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-25 19:12:48.882218 mozregression-5.7.0.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:48.882218 mozregression-5.7.0.dev3/mozregression/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/approx_persist.py
--rw-r--r--   0 runner    (1001) docker     (123)    25458 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/bisector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/bugzilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/build_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/class_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    23215 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)    14034 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/download_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/fetch_build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    21686 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/fetch_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/json_pushes.py
--rw-r--r--   0 runner    (1001) docker     (123)    19190 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/mach_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14567 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/persist_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/pings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/releases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/tc_authenticate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/tempdir.py
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/mozregression/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-25 19:12:48.000000 mozregression-5.7.0.dev3/mozregression/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:12:48.882218 mozregression-5.7.0.dev3/mozregression.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-25 19:12:48.000000 mozregression-5.7.0.dev3/mozregression.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-25 19:12:48.000000 mozregression-5.7.0.dev3/mozregression.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:12:48.000000 mozregression-5.7.0.dev3/mozregression.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 19:12:48.000000 mozregression-5.7.0.dev3/mozregression.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-25 19:12:48.000000 mozregression-5.7.0.dev3/mozregression.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 19:12:48.000000 mozregression-5.7.0.dev3/mozregression.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:12:48.882218 mozregression-5.7.0.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-25 19:11:36.000000 mozregression-5.7.0.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:33:20.552927 mozregression-5.7.1.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/.coveralls.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:33:20.544927 mozregression-5.7.1.dev0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:33:20.544927 mozregression-5.7.1.dev0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/.github/workflows/compile-requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/.github/workflows/deploy-gui.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/.github/workflows/glean-probe-scraper.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/.github/workflows/run-compile-requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-31 14:33:20.548927 mozregression-5.7.1.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:33:20.548927 mozregression-5.7.1.dev0/mozregression/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/approx_persist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25458 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/bisector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/bugzilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/build_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/class_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23215 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14034 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/download_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/fetch_build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21686 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/fetch_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/json_pushes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19190 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/mach_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14567 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/persist_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/pings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/releases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/tc_authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/tempdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/mozregression/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-31 14:33:20.000000 mozregression-5.7.1.dev0/mozregression/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:33:20.548927 mozregression-5.7.1.dev0/mozregression.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-31 14:33:20.000000 mozregression-5.7.1.dev0/mozregression.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-31 14:33:20.000000 mozregression-5.7.1.dev0/mozregression.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:33:20.000000 mozregression-5.7.1.dev0/mozregression.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-31 14:33:20.000000 mozregression-5.7.1.dev0/mozregression.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-31 14:33:20.000000 mozregression-5.7.1.dev0/mozregression.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-31 14:33:20.000000 mozregression-5.7.1.dev0/mozregression.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 14:33:20.552927 mozregression-5.7.1.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-31 14:32:14.000000 mozregression-5.7.1.dev0/setup.py
```

### Comparing `mozregression-5.7.0.dev3/.github/workflows/build.yml` & `mozregression-5.7.1.dev0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/.github/workflows/compile-requirements.yml` & `mozregression-5.7.1.dev0/.github/workflows/compile-requirements.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/.github/workflows/deploy-gui.yml` & `mozregression-5.7.1.dev0/.github/workflows/deploy-gui.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/.github/workflows/deploy.yml` & `mozregression-5.7.1.dev0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/.github/workflows/run-compile-requirements.yml` & `mozregression-5.7.1.dev0/.github/workflows/run-compile-requirements.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/LICENSE` & `mozregression-5.7.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/PKG-INFO` & `mozregression-5.7.1.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozregression
-Version: 5.7.0.dev3
+Version: 5.7.1.dev0
 Summary: Regression range finder for Mozilla nightly builds
 Home-page: http://github.com/mozilla/mozregression
 Author: Mozilla Automation and Tools Team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
 Platform: Any
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `mozregression-5.7.0.dev3/README.md` & `mozregression-5.7.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/approx_persist.py` & `mozregression-5.7.1.dev0/mozregression/approx_persist.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/bisector.py` & `mozregression-5.7.1.dev0/mozregression/bisector.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/branches.py` & `mozregression-5.7.1.dev0/mozregression/branches.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/bugzilla.py` & `mozregression-5.7.1.dev0/mozregression/bugzilla.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/build_info.py` & `mozregression-5.7.1.dev0/mozregression/build_info.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/build_range.py` & `mozregression-5.7.1.dev0/mozregression/build_range.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/class_registry.py` & `mozregression-5.7.1.dev0/mozregression/class_registry.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/cli.py` & `mozregression-5.7.1.dev0/mozregression/cli.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/config.py` & `mozregression-5.7.1.dev0/mozregression/config.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/dates.py` & `mozregression-5.7.1.dev0/mozregression/dates.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/download_manager.py` & `mozregression-5.7.1.dev0/mozregression/download_manager.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/errors.py` & `mozregression-5.7.1.dev0/mozregression/errors.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/fetch_build_info.py` & `mozregression-5.7.1.dev0/mozregression/fetch_build_info.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/fetch_configs.py` & `mozregression-5.7.1.dev0/mozregression/fetch_configs.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/history.py` & `mozregression-5.7.1.dev0/mozregression/history.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/json_pushes.py` & `mozregression-5.7.1.dev0/mozregression/json_pushes.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/launchers.py` & `mozregression-5.7.1.dev0/mozregression/launchers.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/log.py` & `mozregression-5.7.1.dev0/mozregression/log.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/mach_interface.py` & `mozregression-5.7.1.dev0/mozregression/mach_interface.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/main.py` & `mozregression-5.7.1.dev0/mozregression/main.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/metrics.yaml` & `mozregression-5.7.1.dev0/mozregression/metrics.yaml`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/network.py` & `mozregression-5.7.1.dev0/mozregression/network.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/persist_limit.py` & `mozregression-5.7.1.dev0/mozregression/persist_limit.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/pings.yaml` & `mozregression-5.7.1.dev0/mozregression/pings.yaml`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/releases.py` & `mozregression-5.7.1.dev0/mozregression/releases.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/tc_authenticate.py` & `mozregression-5.7.1.dev0/mozregression/tc_authenticate.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/telemetry.py` & `mozregression-5.7.1.dev0/mozregression/telemetry.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/tempdir.py` & `mozregression-5.7.1.dev0/mozregression/tempdir.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression/test_runner.py` & `mozregression-5.7.1.dev0/mozregression/test_runner.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/mozregression.egg-info/PKG-INFO` & `mozregression-5.7.1.dev0/mozregression.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozregression
-Version: 5.7.0.dev3
+Version: 5.7.1.dev0
 Summary: Regression range finder for Mozilla nightly builds
 Home-page: http://github.com/mozilla/mozregression
 Author: Mozilla Automation and Tools Team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
 Platform: Any
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `mozregression-5.7.0.dev3/mozregression.egg-info/SOURCES.txt` & `mozregression-5.7.1.dev0/mozregression.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/pyproject.toml` & `mozregression-5.7.1.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mozregression-5.7.0.dev3/setup.py` & `mozregression-5.7.1.dev0/setup.py`

 * *Files identical despite different names*

