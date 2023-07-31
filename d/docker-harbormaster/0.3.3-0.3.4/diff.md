# Comparing `tmp/docker_harbormaster-0.3.3.tar.gz` & `tmp/docker_harbormaster-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_harbormaster-0.3.3.tar", max compression
+gzip compressed data, was "docker_harbormaster-0.3.4.tar", max compression
```

## Comparing `docker_harbormaster-0.3.3.tar` & `docker_harbormaster-0.3.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    34463 2023-07-23 22:44:54.410761 docker_harbormaster-0.3.3/LICENSE
--rw-r--r--   0        0        0    17954 2023-07-23 22:45:11.969660 docker_harbormaster-0.3.3/README.md
--rw-r--r--   0        0        0        0 2023-07-23 22:44:54.436761 docker_harbormaster-0.3.3/docker_harbormaster/__init__.py
--rwxr-xr-x   0        0        0    28575 2023-07-23 22:44:54.411761 docker_harbormaster-0.3.3/docker_harbormaster/cli.py
--rwxr-xr-x   0        0        0        0 2023-07-23 22:44:54.436761 docker_harbormaster-0.3.3/docker_harbormaster/conftest.py
--rw-r--r--   0        0        0     2777 2023-07-23 22:44:54.411761 docker_harbormaster-0.3.3/docker_harbormaster/utils.py
--rw-r--r--   0        0        0      815 2023-07-23 22:44:54.412761 docker_harbormaster-0.3.3/pyproject.toml
--rw-r--r--   0        0        0    18865 1970-01-01 00:00:00.000000 docker_harbormaster-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    34463 2023-07-31 21:29:03.130341 docker_harbormaster-0.3.4/LICENSE
+-rw-r--r--   0        0        0     3067 2023-07-31 21:29:20.932500 docker_harbormaster-0.3.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-31 21:29:03.158341 docker_harbormaster-0.3.4/docker_harbormaster/__init__.py
+-rwxr-xr-x   0        0        0    28948 2023-07-31 21:29:03.130341 docker_harbormaster-0.3.4/docker_harbormaster/cli.py
+-rwxr-xr-x   0        0        0        0 2023-07-31 21:29:03.158341 docker_harbormaster-0.3.4/docker_harbormaster/conftest.py
+-rw-r--r--   0        0        0     2864 2023-07-31 21:29:03.131341 docker_harbormaster-0.3.4/docker_harbormaster/utils.py
+-rw-r--r--   0        0        0     1038 2023-07-31 21:29:03.132341 docker_harbormaster-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     3935 1970-01-01 00:00:00.000000 docker_harbormaster-0.3.4/PKG-INFO
```

### Comparing `docker_harbormaster-0.3.3/LICENSE` & `docker_harbormaster-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `docker_harbormaster-0.3.3/docker_harbormaster/cli.py` & `docker_harbormaster-0.3.4/docker_harbormaster/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,15 @@
     if any(return_codes):
         raise Exception("Could not stop some containers.")
 
 
 def _run_command_full(
     command: List[Union[str, Path]],
     chdir: Path,
-    environment: Dict[str, str] = None,
+    environment: Optional[Dict[str, str]] = None,
     print_output: bool = False,
 ) -> Tuple[int, bytes]:
     """Run a command and return its exit code, stdout, and stderr."""
     # Include the environment in our command.
     env = os.environ.copy()
     if environment:
         env.update(environment)
@@ -216,15 +216,17 @@
     stdout = b"".join(stdout_list)
     debug(f"Return code: {returncode}")
     os.chdir(wd)
     return (returncode, stdout)
 
 
 def _run_command(
-    command: List[Union[Path, str]], chdir: Path, environment: Dict[str, str] = None
+    command: List[Union[Path, str]],
+    chdir: Path,
+    environment: Optional[Dict[str, str]] = None,
 ) -> int:
     """Run a command and return its exit code."""
     return _run_command_full(command, chdir, environment=environment)[0]
 
 
 def _postproc_command_assuming_exitcode0(status, stdout, errmsg: str) -> int:
     """run_command postprocess to throw an exception of 'errmsg' and 'outout' if status != 0"""
@@ -234,15 +236,15 @@
     return status
 
 
 def _run_command_assuming_exitcode_0(
     command: List[Union[Path, str]],
     chdir: Path,
     errmsg: str,
-    environment: Dict[str, str] = None,
+    environment: Optional[Dict[str, str]] = None,
 ) -> int:
     status, stdout = _run_command_full(command, chdir, environment=environment)
     return _postproc_command_assuming_exitcode0(status, stdout, errmsg)
 
 
 class App:
     def __init__(
@@ -280,14 +282,23 @@
         self.environment.update(
             {
                 key: str(value)
                 for key, value in configuration.get("environment", {}).items()
             }
         )
 
+        # Since Compose now supports env vars in the file, we should insert these there.
+        self.environment.update(
+            {
+                "HM_DATA_DIR": str(self.paths.data_dir),
+                "HM_CACHE_DIR": str(self.paths.cache_dir),
+                "HM_REPO_DIR": str(self.paths.repo_dir),
+            }
+        )
+
         self.replacements: Dict[str, str] = _read_var_file(
             filename=configuration.get("replacements_file", {}),
             base_dir=paths.config_dir,
             app_id=self.id,
         )
         self.replacements.update(
             {
```

### Comparing `docker_harbormaster-0.3.3/docker_harbormaster/utils.py` & `docker_harbormaster-0.3.4/docker_harbormaster/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -44,21 +44,21 @@
         ):
             directory.mkdir(exist_ok=True)
 
     @classmethod
     def for_workdir(cls, workdir: Path, config_dir: Path):
         """Derive the working paths from a base workdir path."""
         return cls(
-            workdir=workdir,
-            config_dir=config_dir,
-            data_dir=workdir / DATA_DIR_NAME,
-            archives_dir=workdir / ARCHIVES_DIR_NAME,
-            repos_dir=workdir / REPOS_DIR_NAME,
-            caches_dir=workdir / CACHES_DIR_NAME,
-            cache_file=workdir / CACHE_FILE_NAME,
+            workdir=workdir.absolute(),
+            config_dir=config_dir.absolute(),
+            data_dir=(workdir / DATA_DIR_NAME).absolute(),
+            archives_dir=(workdir / ARCHIVES_DIR_NAME).absolute(),
+            repos_dir=(workdir / REPOS_DIR_NAME).absolute(),
+            caches_dir=(workdir / CACHES_DIR_NAME).absolute(),
+            cache_file=(workdir / CACHE_FILE_NAME).absolute(),
         )
 
 
 @attr.s(auto_attribs=True)
 class AppPaths:
     workdir: Path
     repo_dir: Path
```

