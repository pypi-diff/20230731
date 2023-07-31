# Comparing `tmp/keycmd-0.4.0.tar.gz` & `tmp/keycmd-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycmd-0.4.0.tar", max compression
+gzip compressed data, was "keycmd-0.5.0.tar", max compression
```

## Comparing `keycmd-0.4.0.tar` & `keycmd-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     6268 2023-07-26 13:31:54.994025 keycmd-0.4.0/README.md
--rw-r--r--   0        0        0       22 2023-07-26 13:31:54.994025 keycmd-0.4.0/keycmd/__init__.py
--rw-r--r--   0        0        0     1199 2023-07-26 13:31:54.994025 keycmd-0.4.0/keycmd/cli.py
--rw-r--r--   0        0        0     2132 2023-07-26 13:31:54.994025 keycmd-0.4.0/keycmd/conf.py
--rw-r--r--   0        0        0      984 2023-07-26 13:31:54.994025 keycmd-0.4.0/keycmd/creds.py
--rw-r--r--   0        0        0      418 2023-07-26 13:31:54.994025 keycmd-0.4.0/keycmd/logs.py
--rw-r--r--   0        0        0     1438 2023-07-26 13:31:54.994025 keycmd-0.4.0/keycmd/shell.py
--rw-r--r--   0        0        0     1069 2023-07-26 13:31:54.994025 keycmd-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6859 1970-01-01 00:00:00.000000 keycmd-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    14053 2023-07-31 11:39:04.925721 keycmd-0.5.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-31 11:39:04.925721 keycmd-0.5.0/keycmd/__init__.py
+-rw-r--r--   0        0        0     1199 2023-07-31 11:39:04.925721 keycmd-0.5.0/keycmd/cli.py
+-rw-r--r--   0        0        0     2838 2023-07-31 11:39:04.925721 keycmd-0.5.0/keycmd/conf.py
+-rw-r--r--   0        0        0      984 2023-07-31 11:39:04.925721 keycmd-0.5.0/keycmd/creds.py
+-rw-r--r--   0        0        0      418 2023-07-31 11:39:04.925721 keycmd-0.5.0/keycmd/logs.py
+-rw-r--r--   0        0        0     1855 2023-07-31 11:39:04.925721 keycmd-0.5.0/keycmd/shell.py
+-rw-r--r--   0        0        0     1069 2023-07-31 11:39:04.929721 keycmd-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    14644 1970-01-01 00:00:00.000000 keycmd-0.5.0/PKG-INFO
```

### Comparing `keycmd-0.4.0/keycmd/cli.py` & `keycmd-0.5.0/keycmd/cli.py`

 * *Files identical despite different names*

### Comparing `keycmd-0.4.0/keycmd/conf.py` & `keycmd-0.5.0/keycmd/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,14 +21,44 @@
 
 def load_pyproj(path):
     """Load [tool.keycmd] from a pyproject.toml file"""
     data = load_toml(path)
     return data.get("tool", {}).get("keycmd", {})
 
 
+def find_file(fname, first_only=True):
+    """Find a file by walking up the filesystem, starting at cwd"""
+    cur = Path.cwd()
+    home = Path.home()
+    results = []
+    while True:
+        candidate = cur / fname
+        if candidate.is_file():
+            hit = candidate.resolve()
+            if first_only:
+                return hit
+            else:
+                results.append(hit)
+        # don't search outside git repositories
+        if (cur / ".git").is_dir():
+            break
+        # stop before searching the home folder
+        if cur.parent == home:
+            break
+        # stop if we can't go up anymore
+        if cur.parent == cur:
+            break
+        cur = cur.parent
+    if not first_only:
+        # return .keycmd files in order in which they should
+        # be loaded and merged
+        results.reverse()
+        return results
+
+
 def defaults():
     """Generate the default config"""
     return {"keys": {}}
 
 
 def merge_conf(a, b):
     """
@@ -46,44 +76,33 @@
 
 
 def load_conf():
     """
     Load merged configuration from the following files:
     - defaults()
     - ~/.keycmd
+    - all .keycmd found while walking file system up from .
     - first pyproject.toml found while walking file system up from .
-    - ./.keycmd
     """
     conf = defaults()
-    cwd = Path.cwd()
 
     # ~/.keycmd
-    fpath = (Path(USERPROFILE).expanduser() / ".keycmd").resolve()
-    if fpath.is_file():
-        vlog(f"loading config file {fpath}")
-        conf = merge_conf(conf, load_toml(fpath))
+    user_keyconf = (Path(USERPROFILE).expanduser() / ".keycmd").resolve()
+    if user_keyconf.is_file():
+        vlog(f"loading config file {user_keyconf}")
+        conf = merge_conf(conf, load_toml(user_keyconf))
+
+    # .keycmd
+    local_keycmds = find_file(".keycmd", first_only=False)
+    for local_keycmd in local_keycmds:
+        vlog(f"loading config file {local_keycmd}")
+        conf = merge_conf(conf, load_toml(local_keycmd))
 
     # pyproject.toml
-    cur = cwd
-    while True:
-        pyproj = cur / "pyproject.toml"
-        if pyproj.is_file():
-            vlog(f"loading config file {pyproj}")
-            conf = merge_conf(conf, load_pyproj(pyproj))
-            break
-        # stop at the boundary of git repositories
-        if (cur / ".git").is_dir():
-            break
-        # stop if we can't go up anymore
-        if cur.parent == cur:
-            break
-        cur = cur.parent
-
-    # ./.keycmd
-    fpath = cwd / ".keycmd"
-    if fpath.is_file():
-        vlog(f"loading config file {fpath}")
-        conf = merge_conf(conf, load_toml(fpath))
+    pyproj = find_file("pyproject.toml")
+    if pyproj is not None:
+        vlog(f"loading config file {pyproj}")
+        conf = merge_conf(conf, load_pyproj(pyproj))
 
     vlog(f"merged config:\n{pformat(conf)}")
 
     return conf
```

### Comparing `keycmd-0.4.0/keycmd/creds.py` & `keycmd-0.5.0/keycmd/creds.py`

 * *Files identical despite different names*

### Comparing `keycmd-0.4.0/keycmd/shell.py` & `keycmd-0.5.0/keycmd/shell.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,44 +5,59 @@
 from sys import exit
 
 from shellingham import detect_shell, ShellDetectionFailure
 
 from .logs import vlog, vwarn
 
 
+USE_SUBPROCESS = False  # exposed for testing
+IS_WINDOWS = os.name == "nt"
+IS_POSIX = os.name == "posix"
+
+
+def exec(args, env):
+    if USE_SUBPROCESS or IS_WINDOWS:
+        # windows does not support process replacement
+        # as well as posix systems do
+        p = run(args, shell=False, env=env)
+        exit(p.returncode)
+    # i know this looks like a bug
+    # but it's a mandatory convention
+    # to pass the process name as the first argument
+    os.execvpe(args[0], args, env)
+
+
 def get_shell():
     """Use shellingham to detect the shell that invoked
     this Python process"""
     try:
         shell_name, shell_path = detect_shell(os.getpid())
     except ShellDetectionFailure:
         vwarn("failed to detect parent process shell, falling back to system default")
-        if os.name == "posix":
+        if IS_POSIX:
             shell_path = os.environ["SHELL"]
-        elif os.name == "nt":
+        elif IS_WINDOWS:
             shell_path = os.environ["COMSPEC"]
         else:
             raise NotImplementedError(f"os {os.name} support not available")
         shell_name = Path(shell_path).name.lower()
     vlog(f"detected shell: {shell_path}")
     return shell_name, shell_path
 
 
 def run_shell(env=None):
     """Open an interactive shell for the user to interact
     with."""
-    _, shell_path = get_shell()
-    vlog("spawning subshell")
-    p = run(shell_path, shell=False, env=env)
-    exit(p.returncode)
+    shell_name, shell_path = get_shell()
+    vlog(f"spawning subshell: {shell_name}")
+    exec([shell_path], env)
 
 
 def run_cmd(cmd, env=None):
     """Run a one-off command in a shell."""
     shell_name, shell_path = get_shell()
     opt = "-c"
     if shell_name == "cmd":
         opt = "/C"
     full_command = [shell_path, opt, *cmd]
     vlog(f"running command: {pformat(full_command)}")
-    p = run(full_command, shell=False, env=env)
-    exit(p.returncode)
+    exec(full_command, env)
```

### Comparing `keycmd-0.4.0/pyproject.toml` & `keycmd-0.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keycmd"
-version = "0.4.0"
+version = "0.5.0"
 description = ""
 authors = ["Korijn van Golen <korijn.vangolen@zimmerbiomet.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
```

