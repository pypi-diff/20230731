# Comparing `tmp/frigobar-1.tar.gz` & `tmp/frigobar-2.tar.gz`

## Comparing `frigobar-1.tar` & `frigobar-2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 frigobar-1/frigobar/__init__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 frigobar-1/frigobar/__main__.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 frigobar-1/frigobar/cli.py
--rw-r--r--   0        0        0     5001 2020-02-02 00:00:00.000000 frigobar-1/frigobar/frigobar.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 frigobar-1/frigobar/downloaders/download_deps.ps1
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 frigobar-1/frigobar/downloaders/download_pip.ps1
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 frigobar-1/frigobar/downloaders/download_python.ps1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frigobar-1/tests/__init__.py
--rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 frigobar-1/tests/test_frigobar.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 frigobar-1/tests/script_folder/another_script.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 frigobar-1/tests/script_folder/requirements.txt
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 frigobar-1/tests/script_folder/script.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frigobar-1/tests/script_folder/data/data
--rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 frigobar-1/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 frigobar-1/license
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 frigobar-1/pyproject.toml
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 frigobar-1/readme.md
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 frigobar-1/PKG-INFO
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 frigobar-2/frigobar/__init__.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 frigobar-2/frigobar/__main__.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 frigobar-2/frigobar/cli.py
+-rw-r--r--   0        0        0     5216 2020-02-02 00:00:00.000000 frigobar-2/frigobar/frigobar.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 frigobar-2/frigobar/downloaders/download_deps.ps1
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 frigobar-2/frigobar/downloaders/download_pip.ps1
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 frigobar-2/frigobar/downloaders/download_python.ps1
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frigobar-2/tests/__init__.py
+-rw-r--r--   0        0        0     8555 2020-02-02 00:00:00.000000 frigobar-2/tests/test_frigobar.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 frigobar-2/tests/script_folder/another_script.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 frigobar-2/tests/script_folder/requirements.txt
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 frigobar-2/tests/script_folder/script.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frigobar-2/tests/script_folder/data/data
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 frigobar-2/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 frigobar-2/license
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 frigobar-2/pyproject.toml
+-rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 frigobar-2/readme.md
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 frigobar-2/PKG-INFO
```

### Comparing `frigobar-1/frigobar/cli.py` & `frigobar-2/frigobar/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,19 @@
         copy_directory=args.copy_directory,
     )
 
 
 def main():
     parser = argparse.ArgumentParser(
         description=(
-            "Distribute Python apps to Windows machines without freezing them."
-            "The resulting distribution will be put in a folder (the 'frigobar') "
-            "that can be copied to any Windows machine. Users should run <script_name>.bat "
-            "to run the script. All the dependencies, including an embeddable version of "
-            "Python, will be downloaded on the first run."
+            "Distribute Python apps to Windows machines without freezing them. The "
+            "resulting distribution will be put in a folder that can be copied to any "
+            'Windows machine. Users should run "<script_name>.bat" to run the script. '
+            "All the dependencies, including an embeddable version of Python, will be "
+            "downloaded on the first run."
         )
     )
     parser.add_argument(
         "script_path", metavar="script-path", help="Path to the script to distribute."
     )
     parser.add_argument(
         "target_directory",
```

### Comparing `frigobar-1/frigobar/frigobar.py` & `frigobar-2/frigobar/frigobar.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,27 +16,29 @@
 def create_frigobar(
     script_path: str,
     target_directory: str = "frigobar",
     python_version: str = "3.11.4",
     requirements_file: str = None,
     copy_directory: bool = False,
 ):
+    script_path = os.path.abspath(script_path)
     if not os.path.exists(target_directory):
         os.mkdir(target_directory)
     elif not os.path.isdir(target_directory):
         raise Exception("Target directory must be a directory")
     elif os.listdir(target_directory):
         raise Exception("Target directory must be empty")
-    python_directory = os.path.join(
-        target_directory, f"python-{python_version}-embed-amd64"
-    )
-
     if not os.path.exists(script_path) or not os.path.isfile(script_path):
         raise Exception(f"Missing script: {script_path}")
 
+    target_directory = os.path.abspath(target_directory)
+
+    requirements_file = (
+        os.path.abspath(requirements_file) if requirements_file else None
+    )
     if requirements_file and (
         not os.path.exists(requirements_file) or not os.path.isfile(requirements_file)
     ):
         raise Exception(f"Missing requirements file: {requirements_file}")
 
     # Add a copy of the script to frigobar
     script_dir = os.path.join(target_directory, "script")
@@ -67,14 +69,17 @@
     os.mkdir(downloaders_dir)
     for script in downloader_scripts:
         if not os.path.exists(script):
             raise Exception(f"Missing script: {script}")
         shutil.copy(script, downloaders_dir)
 
     # Create bat file
+    python_directory = os.path.join(
+        target_directory, f"python-{python_version}-embed-amd64"
+    )
     rel_target_directory = os.path.relpath(target_directory, target_directory)
     rel_python_directory = os.path.relpath(python_directory, target_directory)
     rel_pip_path = os.path.relpath(
         os.path.join(python_directory, "Scripts", "pip.exe"), target_directory
     )
     rel_script_path = os.path.relpath(
         os.path.join(script_dir, os.path.basename(script_path)), target_directory
```

### Comparing `frigobar-1/frigobar/downloaders/download_pip.ps1` & `frigobar-2/frigobar/downloaders/download_pip.ps1`

 * *Files identical despite different names*

### Comparing `frigobar-1/frigobar/downloaders/download_python.ps1` & `frigobar-2/frigobar/downloaders/download_python.ps1`

 * *Files identical despite different names*

### Comparing `frigobar-1/.gitignore` & `frigobar-2/.gitignore`

 * *Files identical despite different names*

### Comparing `frigobar-1/license` & `frigobar-2/license`

 * *Files identical despite different names*

### Comparing `frigobar-1/pyproject.toml` & `frigobar-2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "frigobar"
-version = "1"
+version = "2"
 description = "Distribute Python apps to Windows machines without freezing them."
 authors = [
     {name="ubalklen", email="42127323+ubalklen@users.noreply.github.com"},
 ]
 readme = "readme.md"
 
 [project.urls]
```

### Comparing `frigobar-1/PKG-INFO` & `frigobar-2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frigobar
-Version: 1
+Version: 2
 Summary: Distribute Python apps to Windows machines without freezing them.
 Project-URL: Homepage, https://github.com/ubalklen/my_package
 Project-URL: Bug Tracker, https://github.com/ubalklen/my_package/issues
 Author-email: ubalklen <42127323+ubalklen@users.noreply.github.com>
 License-File: license
 Description-Content-Type: text/markdown
 
@@ -20,15 +20,33 @@
 ## Installation
 ```
 pip install frigobar
 ```
 
 ## Options
 ```
-frigobar --help
+> frigobar --help
+usage: frigobar [-h] [-r REQUIREMENTS_FILE] [-p PYTHON_VERSION] [--copy-directory] script-path [target-directory]
+
+Distribute Python apps to Windows machines without freezing them. The resulting distribution will be put in a folder that   
+can be copied to any Windows machine. Users should run "<script_name>.bat" to run the script. All the dependencies,
+including an embeddable version of Python, will be downloaded on the first run.
+
+positional arguments:
+  script-path           Path to the script to distribute.
+  target-directory      Folder where the distribution will be put. Defaults to 'frigobar'.
+
+options:
+  -h, --help            show this help message and exit
+  -r REQUIREMENTS_FILE, --requirements-file REQUIREMENTS_FILE
+                        Path to a requirements file that lists the dependencies of the script.
+  -p PYTHON_VERSION, --python-version PYTHON_VERSION, --python PYTHON_VERSION
+                        Python version, in X.Y.Z format, that the distribution should use.The version must be available as  
+                        an embeddable package on https://www.python.org/downloads/windows/. Defaults to 3.11.4.
+  --copy-directory      Copy the contents of the script directory to the distribution.
 ```
 
 ## Rationale
 A common technique to distribute Python apps is to "freeze" them using tools like [PyInstaller](https://pyinstaller.org/) or [cx_Freeze](https://cx-freeze.readthedocs.io/). These freezers create a standalone executable that contains your app and all its dependencies. This is a workable solution, but it has two main drawbacks:
 
 1. The resulting frozen app is often huge. It's not uncommon to see a simple app taking MBs of space.
 2. Because dependence resolution is hard, the frozen app may contain more or less dependencies than it needs. Less dependencies lead to dread "working-app-that-stop-working-when-you-freeze-it" situations. Unnecessary dependencies lead to bloated apps.
```

