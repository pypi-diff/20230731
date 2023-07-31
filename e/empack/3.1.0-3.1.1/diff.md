# Comparing `tmp/empack-3.1.0.tar.gz` & `tmp/empack-3.1.1.tar.gz`

## Comparing `empack-3.1.0.tar` & `empack-3.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 empack-3.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 empack-3.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 empack-3.1.0/ci_env.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 empack-3.1.0/setup.py
--rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 empack-3.1.0/config/empack_config.yaml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 empack-3.1.0/empack/__init__.py
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 empack-3.1.0/empack/file_patterns.py
--rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 empack-3.1.0/empack/filter_env.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 empack-3.1.0/empack/micromamba_wrapper.py
--rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 empack-3.1.0/empack/pack.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 empack-3.1.0/empack/repodata.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 empack-3.1.0/empack/tar_utils.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 empack-3.1.0/empack/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 empack-3.1.0/empack/cli/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 empack-3.1.0/empack/cli/app.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 empack-3.1.0/empack/cli/err.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 empack-3.1.0/empack/cli/main.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 empack-3.1.0/empack/cli/pack.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 empack-3.1.0/empack/cli/repodata.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 empack-3.1.0/empack/cli/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 empack-3.1.0/tests/__init__.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 empack-3.1.0/tests/conftest.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 empack-3.1.0/tests/empack_test_config.yaml
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 empack-3.1.0/tests/empack_test_extra_config.yaml
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 empack-3.1.0/tests/test_cli.py
--rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 empack-3.1.0/tests/test_filter.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 empack-3.1.0/tests/test_integration.py
--rw-r--r--   0        0        0     6456 2020-02-02 00:00:00.000000 empack-3.1.0/tests/test_pack.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 empack-3.1.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 empack-3.1.0/LICENSE
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 empack-3.1.0/README.md
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 empack-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 empack-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 empack-3.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 empack-3.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 empack-3.1.1/ci_env.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 empack-3.1.1/setup.py
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 empack-3.1.1/config/empack_config.yaml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 empack-3.1.1/empack/__init__.py
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 empack-3.1.1/empack/file_patterns.py
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 empack-3.1.1/empack/filter_env.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 empack-3.1.1/empack/micromamba_wrapper.py
+-rw-r--r--   0        0        0     8333 2020-02-02 00:00:00.000000 empack-3.1.1/empack/pack.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 empack-3.1.1/empack/repodata.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 empack-3.1.1/empack/tar_utils.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 empack-3.1.1/empack/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 empack-3.1.1/empack/cli/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 empack-3.1.1/empack/cli/app.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 empack-3.1.1/empack/cli/err.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 empack-3.1.1/empack/cli/main.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 empack-3.1.1/empack/cli/pack.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 empack-3.1.1/empack/cli/repodata.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 empack-3.1.1/empack/cli/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 empack-3.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 empack-3.1.1/tests/conftest.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 empack-3.1.1/tests/empack_test_config.yaml
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 empack-3.1.1/tests/empack_test_extra_config.yaml
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 empack-3.1.1/tests/test_cli.py
+-rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 empack-3.1.1/tests/test_filter.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 empack-3.1.1/tests/test_integration.py
+-rw-r--r--   0        0        0     6456 2020-02-02 00:00:00.000000 empack-3.1.1/tests/test_pack.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 empack-3.1.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 empack-3.1.1/LICENSE
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 empack-3.1.1/README.md
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 empack-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 empack-3.1.1/PKG-INFO
```

### Comparing `empack-3.1.0/.pre-commit-config.yaml` & `empack-3.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `empack-3.1.0/config/empack_config.yaml` & `empack-3.1.1/config/empack_config.yaml`

 * *Files identical despite different names*

### Comparing `empack-3.1.0/empack/file_patterns.py` & `empack-3.1.1/empack/file_patterns.py`

 * *Files identical despite different names*

### Comparing `empack-3.1.0/empack/filter_env.py` & `empack-3.1.1/empack/filter_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 import shutil
 from pathlib import Path
 
 
 def iterate_pip_pkg_record(env_prefix):
     # Find all RECORD files for .dist-info folders for which INSTALLER is "pip"
     # Resolve site-packages directory, ignoring the python3.1/ symlink
+    prefix = Path(env_prefix).resolve()
+
     site_packages = [
         site_package
-        for site_package in Path(env_prefix).resolve().glob("lib/python*/site-packages")
+        for site_package in prefix.glob("lib/python*/site-packages")
         if "python3.1" not in site_package.parts
     ]
     if not site_packages:
         return []
     site_packages = site_packages[0]
-    relative_site_packages = site_packages.relative_to(env_prefix)
+    relative_site_packages = site_packages.relative_to(prefix)
 
     packages_dist_info = Path(site_packages).resolve().glob("*.dist-info")
 
     for dist_info in packages_dist_info:
         if not (dist_info / "INSTALLER").exists():
             continue
```

### Comparing `empack-3.1.0/empack/micromamba_wrapper.py` & `empack-3.1.1/empack/micromamba_wrapper.py`

 * *Files identical despite different names*

### Comparing `empack-3.1.0/empack/pack.py` & `empack-3.1.1/empack/pack.py`

 * *Files identical despite different names*

### Comparing `empack-3.1.0/empack/repodata.py` & `empack-3.1.1/empack/repodata.py`

 * *Files identical despite different names*

### Comparing `empack-3.1.0/empack/tar_utils.py` & `empack-3.1.1/empack/tar_utils.py`

 * *Files identical despite different names*

### Comparing `empack-3.1.0/empack/cli/pack.py` & `empack-3.1.1/empack/cli/pack.py`

 * *Files identical despite different names*

### Comparing `empack-3.1.0/empack/cli/repodata.py` & `empack-3.1.1/empack/cli/repodata.py`

 * *Files identical despite different names*

### Comparing `empack-3.1.0/tests/conftest.py` & `empack-3.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `empack-3.1.0/tests/empack_test_config.yaml` & `empack-3.1.1/tests/empack_test_config.yaml`

 * *Files identical despite different names*

### Comparing `empack-3.1.0/tests/test_cli.py` & `empack-3.1.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `empack-3.1.0/tests/test_filter.py` & `empack-3.1.1/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `empack-3.1.0/tests/test_integration.py` & `empack-3.1.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `empack-3.1.0/tests/test_pack.py` & `empack-3.1.1/tests/test_pack.py`

 * *Files identical despite different names*

### Comparing `empack-3.1.0/.gitignore` & `empack-3.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `empack-3.1.0/LICENSE` & `empack-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `empack-3.1.0/README.md` & `empack-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `empack-3.1.0/pyproject.toml` & `empack-3.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `empack-3.1.0/PKG-INFO` & `empack-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empack
-Version: 3.1.0
+Version: 3.1.1
 Summary: empack emscripten+boa
 Project-URL: Homepage, https://github.com/emscripten-forge/empack
 Author-email: Thorsten Beier <derthorstenbeier@gmail.com>
 License: 
         MIT License
         
         Copyright (c) 2022, Thorsten Beier
```

