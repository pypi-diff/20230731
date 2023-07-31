# Comparing `tmp/pyclang-0.2.3.tar.gz` & `tmp/pyclang-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyclang-0.2.3.tar", last modified: Fri Feb 17 04:35:01 2023, max compression
+gzip compressed data, was "dist/pyclang-0.3.0.tar", last modified: Mon Jul 31 17:37:22 2023, max compression
```

## Comparing `pyclang-0.2.3.tar` & `pyclang-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 04:35:01.000000 pyclang-0.2.3/
--rw-r--r--   0 root         (0) root         (0)     2469 2023-02-17 04:35:01.000000 pyclang-0.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1398 2023-02-17 04:34:51.000000 pyclang-0.2.3/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-17 04:35:01.000000 pyclang-0.2.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 04:35:01.000000 pyclang-0.2.3/pyclang.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2469 2023-02-17 04:35:01.000000 pyclang-0.2.3/pyclang.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       72 2023-02-17 04:35:01.000000 pyclang-0.2.3/pyclang.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      390 2023-02-17 04:35:01.000000 pyclang-0.2.3/pyclang.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-02-17 04:35:01.000000 pyclang-0.2.3/pyclang.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-02-17 04:35:01.000000 pyclang-0.2.3/pyclang.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-17 04:35:01.000000 pyclang-0.2.3/pyclang.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1094 2023-02-17 04:34:51.000000 pyclang-0.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1674 2023-02-17 04:34:51.000000 pyclang-0.2.3/README.md
--rw-r--r--   0 root         (0) root         (0)      101 2023-02-17 04:34:51.000000 pyclang-0.2.3/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 04:35:01.000000 pyclang-0.2.3/pyclang/
--rw-r--r--   0 root         (0) root         (0)     3178 2023-02-17 04:34:51.000000 pyclang-0.2.3/pyclang/idf_extension.py
--rw-r--r--   0 root         (0) root         (0)    15561 2023-02-17 04:34:51.000000 pyclang-0.2.3/pyclang/runner.py
--rw-r--r--   0 root         (0) root         (0)       56 2023-02-17 04:34:51.000000 pyclang-0.2.3/pyclang/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-02-17 04:34:51.000000 pyclang-0.2.3/pyclang/cli_ext.py
--rw-r--r--   0 root         (0) root         (0)     1781 2023-02-17 04:34:51.000000 pyclang-0.2.3/pyclang/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 04:35:01.000000 pyclang-0.2.3/pyclang/scripts/
--rw-r--r--   0 root         (0) root         (0)     1266 2023-02-17 04:34:51.000000 pyclang-0.2.3/pyclang/scripts/idf_clang_tidy.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-17 04:34:51.000000 pyclang-0.2.3/pyclang/scripts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 17:37:22.000000 pyclang-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 17:37:22.000000 pyclang-0.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2469 2023-07-31 17:37:22.000000 pyclang-0.3.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 17:37:22.000000 pyclang-0.3.0/pyclang.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2469 2023-07-31 17:37:22.000000 pyclang-0.3.0/pyclang.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-31 17:37:22.000000 pyclang-0.3.0/pyclang.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      390 2023-07-31 17:37:22.000000 pyclang-0.3.0/pyclang.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-31 17:37:22.000000 pyclang-0.3.0/pyclang.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 17:37:22.000000 pyclang-0.3.0/pyclang.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2023-07-31 17:37:22.000000 pyclang-0.3.0/pyclang.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-07-31 17:37:09.000000 pyclang-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-31 17:37:09.000000 pyclang-0.3.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-07-31 17:37:09.000000 pyclang-0.3.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-31 17:37:09.000000 pyclang-0.3.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 17:37:22.000000 pyclang-0.3.0/pyclang/
+-rw-r--r--   0 root         (0) root         (0)    16089 2023-07-31 17:37:09.000000 pyclang-0.3.0/pyclang/runner.py
+-rw-r--r--   0 root         (0) root         (0)     2325 2023-07-31 17:37:09.000000 pyclang-0.3.0/pyclang/cli_ext.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 17:37:22.000000 pyclang-0.3.0/pyclang/scripts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 17:37:09.000000 pyclang-0.3.0/pyclang/scripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1266 2023-07-31 17:37:09.000000 pyclang-0.3.0/pyclang/scripts/idf_clang_tidy.py
+-rw-r--r--   0 root         (0) root         (0)     3503 2023-07-31 17:37:09.000000 pyclang-0.3.0/pyclang/idf_extension.py
+-rw-r--r--   0 root         (0) root         (0)     1900 2023-07-31 17:37:09.000000 pyclang-0.3.0/pyclang/utils.py
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-31 17:37:09.000000 pyclang-0.3.0/pyclang/__init__.py
```

### Comparing `pyclang-0.2.3/PKG-INFO` & `pyclang-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclang
-Version: 0.2.3
+Version: 0.3.0
 Summary: A python clang-tidy runner
 Home-page: UNKNOWN
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `pyclang-0.2.3/setup.py` & `pyclang-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyclang-0.2.3/pyclang.egg-info/PKG-INFO` & `pyclang-0.3.0/pyclang.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclang
-Version: 0.2.3
+Version: 0.3.0
 Summary: A python clang-tidy runner
 Home-page: UNKNOWN
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `pyclang-0.2.3/LICENSE` & `pyclang-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclang-0.2.3/README.md` & `pyclang-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyclang-0.2.3/pyclang/idf_extension.py` & `pyclang-0.3.0/pyclang/idf_extension.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,20 @@
                     },
                     {
                         'names': ['--exclude-paths'],
                         'multiple': True,
                         'help': 'exclude extra files besides of the project dir. '
                         'This option can be used for multiple times.',
                     },
+                    {
+                        'names': ['--exit-code'],
+                        'help': 'Exit with code based on the results of the code analysis. '
+                        'By default, exit code reflects the success of running the tool only.',
+                        'is_flag': True,
+                    },
                 ],
             },
             'clang-html-report': {
                 'callback': call_runner,
                 'help': 'generate html report to "html_report" folder by reading "warnings.txt" '
                 '(may take a few minutes). '
                 'This feature requires extra dependency "codereport". '
```

### Comparing `pyclang-0.2.3/pyclang/runner.py` & `pyclang-0.3.0/pyclang/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,34 +5,43 @@
 import sys
 import shlex
 from datetime import datetime
 from functools import wraps
 
 import typing as t
 
-from .utils import to_path, run_cmd
+from .utils import to_path, run_cmd, to_realpath
 
 
 def _remove_prefix(s: str, prefix: str) -> str:
     while s.startswith(prefix):
         s = s[len(prefix) :]
     return s
 
 
-def _get_real_path(s: str) -> str:
+def _is_exe(filepath: str) -> bool:
+    if sys.platform == 'win32' and os.path.splitext(filepath)[-1].lower() == '.exe':
+        return True
+
+    return False
+
+
+def _get_call_cmd(filepath: str) -> t.List[str]:
+    realpath = to_realpath(filepath)
+
     # if s is a file
-    if os.path.isfile(os.path.realpath(s)):
-        return os.path.realpath(s)
+    if os.path.isfile(realpath):
+        return [realpath] if _is_exe(realpath) else [sys.executable, realpath]
 
     # if s is an executable in $PATH
-    full_path = shutil.which(s)
-    if not full_path:
-        raise FileNotFoundError(f'{s} not found in your PATH')
+    fullpath = shutil.which(filepath)
+    if not fullpath:
+        raise FileNotFoundError(f'{filepath} not found in your PATH')
 
-    return full_path
+    return [fullpath] if _is_exe(fullpath) else [sys.executable, fullpath]
 
 
 class Runner:
     """
     Should be used with:
     >> runner = Runner(...args, ...kwargs)
     >> runner = runner.idf_configure().run_clang_tidy().normalize()
@@ -141,21 +150,25 @@
 
         # assign the rest arguments
         for k, v in kwargs.items():
             setattr(self, str(k), v)
 
         self._call_chain = []
 
+        self.expect_returncode = [0]
+        if not kwargs.get('exit_code', False):
+            self.expect_returncode.append(1)
+
     @property
-    def idf_py(self) -> str:
-        return _get_real_path('idf.py')
+    def idf_py_cmd(self) -> t.List[str]:
+        return _get_call_cmd('idf.py')
 
     @property
-    def run_clang_tidy_py(self) -> str:
-        return _get_real_path(self._run_clang_tidy_py)
+    def run_clang_tidy_py_cmd(self) -> t.List[str]:
+        return _get_call_cmd(self._run_clang_tidy_py)
 
     def _run(self, folder, log_fs, output_dir):
         for func in self._call_chain:
             func(folder, log_fs, output_dir)
 
     def __call__(self):
         """
@@ -220,15 +233,15 @@
         """
         Run "idf.py reconfigure" to get the compiled commands
         """
         folder = args[0]
         log_fs = args[1]
 
         run_cmd(
-            [sys.executable, self.idf_py, '-B', self.build_dir, 'reconfigure'],
+            self.idf_py_cmd + ['-B', self.build_dir, 'reconfigure'],
             log_stream=log_fs,
             cwd=folder,
         )
 
     @chain
     def remove_command_flags(self, *args):
         folder = args[0]
@@ -308,29 +321,31 @@
     def run_clang_tidy(self, *args):
         folder = args[0]
         log_fs = args[1]
         output_dir = args[2]
 
         warn_file = os.path.join(output_dir, self.WARN_FILENAME)
 
-        cmd = [
-            sys.executable,
-            self.run_clang_tidy_py,
+        cmd = self.run_clang_tidy_py_cmd + [
             '-p',
             self.build_dir,
         ]
         if self.clang_extra_args:
             cmd.extend(shlex.split(self.clang_extra_args))
 
         cmd.append(' '.join(self.check_files_regex))
 
         with open(warn_file, 'w') as fw:
             # clang-tidy would return 1 when found issue, ignore this return code
             run_cmd(
-                cmd, log_stream=log_fs, stream=fw, cwd=folder, expect_returncode=[0, 1]
+                cmd,
+                log_stream=log_fs,
+                stream=fw,
+                cwd=folder,
+                expect_returncode=self.expect_returncode,
             )
 
         log_fs.write(f'clang-tidy report generated: {warn_file}\n')
 
     @chain
     def check_limits(self, *args):
         log_fs = args[1]
@@ -434,15 +449,15 @@
             shutil.rmtree(html_report_folder)
 
         known_issue = run_cmd(
             ['codereport', '--prefix', self.base_dir, report_json_fn, 'html_report'],
             log_stream=log_fs,
             cwd=output_dir,
             ignore_error='AssertionError: No existing files found',
-            expect_returncode=[0, 1],
+            expect_returncode=self.expect_returncode,
         )
         if known_issue:
             log_fs.write('No issue found\n')
         else:
             log_fs.write(
                 f'Please open {output_dir}/html_report/index.html to view the report\n'
             )
```

### Comparing `pyclang-0.2.3/pyclang/cli_ext.py` & `pyclang-0.3.0/pyclang/cli_ext.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,19 @@
     help='where the newly generated files locates, will be placed under each "dirs" item if not specified',
 )
 common_args.add_argument(
     '--log-path',
     type=os.path.realpath,
     help='where the log files will be write to. will use stdout if not specified',
 )
+common_args.add_argument(
+    '--exit-code',
+    action='store_true',
+    help='Exit with code based on the results of the code analysis. By default, exit code reflects the success of running the tool only.',
+)
 
 idf_specific_args = argparse.ArgumentParser(add_help=False)
 idf_specific_args.add_argument(
     '--limit-file', help='definitions of ignore checks and files/dirs to skip'
 )
 idf_specific_args.add_argument(
     '--xtensa-include-dir',
```

### Comparing `pyclang-0.2.3/pyclang/utils.py` & `pyclang-0.3.0/pyclang/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 import sys
 from pathlib import Path
 
 import typing as t
 
 
 def to_path(*args: str) -> Path:
-    return Path(os.path.join(*args)).resolve()
+    return Path(os.path.expanduser(os.path.join(*args))).resolve()
+
+
+def to_realpath(filepath: str) -> str:
+    return os.path.realpath(os.path.expanduser(filepath))
 
 
 def to_str(bytes_str: t.AnyStr) -> str:
     if isinstance(bytes_str, bytes):
         return bytes_str.decode('utf-8', errors='ignore')
     return bytes_str
```

### Comparing `pyclang-0.2.3/pyclang/scripts/idf_clang_tidy.py` & `pyclang-0.3.0/pyclang/scripts/idf_clang_tidy.py`

 * *Files identical despite different names*

