# Comparing `tmp/frigobar-2.tar.gz` & `tmp/frigobar-3.tar.gz`

## Comparing `frigobar-2.tar` & `frigobar-3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 frigobar-2/frigobar/__init__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 frigobar-2/frigobar/__main__.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 frigobar-2/frigobar/cli.py
--rw-r--r--   0        0        0     5216 2020-02-02 00:00:00.000000 frigobar-2/frigobar/frigobar.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 frigobar-2/frigobar/downloaders/download_deps.ps1
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 frigobar-2/frigobar/downloaders/download_pip.ps1
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 frigobar-2/frigobar/downloaders/download_python.ps1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frigobar-2/tests/__init__.py
--rw-r--r--   0        0        0     8555 2020-02-02 00:00:00.000000 frigobar-2/tests/test_frigobar.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 frigobar-2/tests/script_folder/another_script.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 frigobar-2/tests/script_folder/requirements.txt
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 frigobar-2/tests/script_folder/script.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frigobar-2/tests/script_folder/data/data
--rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 frigobar-2/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 frigobar-2/license
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 frigobar-2/pyproject.toml
--rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 frigobar-2/readme.md
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 frigobar-2/PKG-INFO
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 frigobar-3/frigobar/__init__.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 frigobar-3/frigobar/__main__.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 frigobar-3/frigobar/cli.py
+-rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 frigobar-3/frigobar/frigobar.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 frigobar-3/frigobar/downloaders/download_deps.ps1
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 frigobar-3/frigobar/downloaders/download_pip.ps1
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 frigobar-3/frigobar/downloaders/download_python.ps1
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frigobar-3/tests/__init__.py
+-rw-r--r--   0        0        0    10805 2020-02-02 00:00:00.000000 frigobar-3/tests/test_frigobar.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 frigobar-3/tests/script_folder/another_script.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 frigobar-3/tests/script_folder/requirements.txt
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 frigobar-3/tests/script_folder/script.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frigobar-3/tests/script_folder/data/data
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 frigobar-3/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 frigobar-3/license
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 frigobar-3/pyproject.toml
+-rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 frigobar-3/readme.md
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 frigobar-3/PKG-INFO
```

### Comparing `frigobar-2/frigobar/cli.py` & `frigobar-3/frigobar/cli.py`

 * *Files identical despite different names*

### Comparing `frigobar-2/frigobar/frigobar.py` & `frigobar-3/frigobar/frigobar.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,24 @@
 
     # Add a copy of the script to frigobar
     script_dir = os.path.join(target_directory, "script")
     os.mkdir(script_dir)
     if not copy_directory:
         shutil.copy(script_path, script_dir)
     else:
-        shutil.copytree(os.path.dirname(script_path), script_dir, dirs_exist_ok=True)
+
+        def ignore_target_dir(dir, contents):
+            return [c for c in contents if os.path.join(dir, c) == target_directory]
+
+        shutil.copytree(
+            os.path.dirname(script_path),
+            script_dir,
+            dirs_exist_ok=True,
+            ignore=ignore_target_dir,
+        )
 
     # Add a copy of the requirements file to frigobar
     if requirements_file:
         shutil.copy(requirements_file, script_dir)
 
     # Add a copy of the downloaders to frigobar
     downloaders_dir = os.path.join(os.path.dirname(__file__), "downloaders")
```

### Comparing `frigobar-2/frigobar/downloaders/download_pip.ps1` & `frigobar-3/frigobar/downloaders/download_pip.ps1`

 * *Files identical despite different names*

### Comparing `frigobar-2/frigobar/downloaders/download_python.ps1` & `frigobar-3/frigobar/downloaders/download_python.ps1`

 * *Files identical despite different names*

### Comparing `frigobar-2/tests/test_frigobar.py` & `frigobar-3/tests/test_frigobar.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,22 @@
 @pytest.fixture(autouse=True)
 def delete_test_frigobar():
     shutil.rmtree(target_dir, ignore_errors=True)
     yield
     shutil.rmtree(target_dir, ignore_errors=True)
 
 
+@pytest.fixture
+def target_dir_inside_script_dir():
+    new_target_dir = path.join(test_dir, "script_folder", "test_frigobar")
+    shutil.rmtree(new_target_dir, ignore_errors=True)
+    yield new_target_dir
+    shutil.rmtree(new_target_dir, ignore_errors=True)
+
+
 def test_create_frigobar_abs_script_path():
     frigobar.create_frigobar(
         script_path=script_path,
         target_directory=target_dir,
         requirements_file=requirements_file,
         python_version=python_version,
     )
@@ -71,15 +79,15 @@
 powershell -ExecutionPolicy Bypass -File "%~dp0downloaders\download_python.ps1" -Version 3.8.5 -TargetDirectory "."
 powershell -ExecutionPolicy Bypass -File "%~dp0downloaders\download_pip.ps1" -TargetDirectory "python-3.8.5-embed-amd64"
 powershell -ExecutionPolicy Bypass -File "%~dp0downloaders\download_deps.ps1" -RequirementsFile "script\requirements.txt" -PipPath "python-3.8.5-embed-amd64\Scripts\pip.exe"
 "%~dp0/python-3.8.5-embed-amd64/python.exe" "script\script.py"'''
         )
 
 
-def test_create_frigobar_with_folder():
+def test_create_frigobar_copy_script_dir():
     frigobar.create_frigobar(
         script_path=script_path,
         target_directory=target_dir,
         requirements_file=requirements_file,
         python_version=python_version,
         copy_directory=True,
     )
@@ -101,15 +109,15 @@
 powershell -ExecutionPolicy Bypass -File "%~dp0downloaders\download_python.ps1" -Version 3.8.5 -TargetDirectory "."
 powershell -ExecutionPolicy Bypass -File "%~dp0downloaders\download_pip.ps1" -TargetDirectory "python-3.8.5-embed-amd64"
 powershell -ExecutionPolicy Bypass -File "%~dp0downloaders\download_deps.ps1" -RequirementsFile "script\requirements.txt" -PipPath "python-3.8.5-embed-amd64\Scripts\pip.exe"
 "%~dp0/python-3.8.5-embed-amd64/python.exe" "script\script.py"'''
         )
 
 
-def test_create_frigobar_with_folder_and_rel_script_path():
+def test_create_frigobar_copy_script_dir_and_rel_script_path():
     os.chdir(os.path.dirname(script_path))
     script_rel_path = os.path.basename(script_path)
     frigobar.create_frigobar(
         script_path=script_rel_path,
         target_directory=target_dir,
         requirements_file=requirements_file,
         python_version=python_version,
@@ -130,14 +138,56 @@
         assert (
             f.read()
             == r'''powershell Unblock-File -Path '%~dp0downloaders\download_python.ps1'
 powershell -ExecutionPolicy Bypass -File "%~dp0downloaders\download_python.ps1" -Version 3.8.5 -TargetDirectory "."
 powershell -ExecutionPolicy Bypass -File "%~dp0downloaders\download_pip.ps1" -TargetDirectory "python-3.8.5-embed-amd64"
 powershell -ExecutionPolicy Bypass -File "%~dp0downloaders\download_deps.ps1" -RequirementsFile "script\requirements.txt" -PipPath "python-3.8.5-embed-amd64\Scripts\pip.exe"
 "%~dp0/python-3.8.5-embed-amd64/python.exe" "script\script.py"'''
+        )
+
+
+def test_create_frigobar_target_dir_inside_script_dir(target_dir_inside_script_dir):
+    frigobar.create_frigobar(
+        script_path=script_path,
+        target_directory=target_dir_inside_script_dir,
+        requirements_file=requirements_file,
+        python_version=python_version,
+        copy_directory=True,
+    )
+
+    assert path.exists(path.join(target_dir_inside_script_dir, "script", "script.py"))
+    assert path.exists(
+        path.join(target_dir_inside_script_dir, "script", "another_script.py")
+    )
+    assert path.exists(path.join(target_dir_inside_script_dir, "script", "data"))
+    assert path.exists(
+        path.join(target_dir_inside_script_dir, "script", "data", "data")
+    )
+    assert path.exists(
+        path.join(target_dir_inside_script_dir, "script", "requirements.txt")
+    )
+    assert path.exists(
+        path.join(target_dir_inside_script_dir, "downloaders", "download_python.ps1")
+    )
+    assert path.exists(
+        path.join(target_dir_inside_script_dir, "downloaders", "download_pip.ps1")
+    )
+    assert path.exists(
+        path.join(target_dir_inside_script_dir, "downloaders", "download_deps.ps1")
+    )
+    assert path.exists(path.join(target_dir_inside_script_dir, "script.bat"))
+
+    with open(path.join(target_dir_inside_script_dir, "script.bat"), "r") as f:
+        assert (
+            f.read()
+            == r'''powershell Unblock-File -Path '%~dp0downloaders\download_python.ps1'
+powershell -ExecutionPolicy Bypass -File "%~dp0downloaders\download_python.ps1" -Version 3.8.5 -TargetDirectory "."
+powershell -ExecutionPolicy Bypass -File "%~dp0downloaders\download_pip.ps1" -TargetDirectory "python-3.8.5-embed-amd64"
+powershell -ExecutionPolicy Bypass -File "%~dp0downloaders\download_deps.ps1" -RequirementsFile "script\requirements.txt" -PipPath "python-3.8.5-embed-amd64\Scripts\pip.exe"
+"%~dp0/python-3.8.5-embed-amd64/python.exe" "script\script.py"'''
         )
 
 
 def test_create_frigobar_without_reqs():
     frigobar.create_frigobar(
         script_path=script_path,
         target_directory=target_dir,
```

### Comparing `frigobar-2/.gitignore` & `frigobar-3/.gitignore`

 * *Files identical despite different names*

### Comparing `frigobar-2/license` & `frigobar-3/license`

 * *Files identical despite different names*

### Comparing `frigobar-2/pyproject.toml` & `frigobar-3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "frigobar"
-version = "2"
+version = "3"
 description = "Distribute Python apps to Windows machines without freezing them."
 authors = [
     {name="ubalklen", email="42127323+ubalklen@users.noreply.github.com"},
 ]
 readme = "readme.md"
 
 [project.urls]
```

### Comparing `frigobar-2/readme.md` & `frigobar-3/readme.md`

 * *Files identical despite different names*

### Comparing `frigobar-2/PKG-INFO` & `frigobar-3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frigobar
-Version: 2
+Version: 3
 Summary: Distribute Python apps to Windows machines without freezing them.
 Project-URL: Homepage, https://github.com/ubalklen/my_package
 Project-URL: Bug Tracker, https://github.com/ubalklen/my_package/issues
 Author-email: ubalklen <42127323+ubalklen@users.noreply.github.com>
 License-File: license
 Description-Content-Type: text/markdown
```

