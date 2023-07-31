# Comparing `tmp/jupyterlite_core-0.1.0rc0.tar.gz` & `tmp/jupyterlite_core-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Apr  1 06:43:15 2023, max compression
+gzip compressed data, last modified: Mon Jul 31 13:00:28 2023, max compression
```

## Comparing `jupyterlite_core-0.1.0rc0.tar` & `jupyterlite_core-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0       70 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/__init__.py
--rw-r--r--   0        0        0       81 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/__main__.py
--rw-r--r--   0        0        0    10543 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/app.py
--rw-r--r--   0        0        0     8940 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/config.py
--rw-r--r--   0        0        0     4809 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/constants.py
--rw-r--r--   0        0        0  7436742 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/jupyterlite-app-0.1.0-rc.0.tgz
--rw-r--r--   0        0        0     5532 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/manager.py
--rw-r--r--   0        0        0      691 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/optional.py
--rw-r--r--   0        0        0      665 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/trait_types.py
--rw-r--r--   0        0        0     3020 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/__init__.py
--rw-r--r--   0        0        0     5644 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/archive.py
--rw-r--r--   0        0        0    13904 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/base.py
--rw-r--r--   0        0        0     8526 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/contents.py
--rw-r--r--   0        0        0    11685 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/federated_extensions.py
--rw-r--r--   0        0        0      153 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/icons.py
--rw-r--r--   0        0        0     2813 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/lite.py
--rw-r--r--   0        0        0     4589 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/mathjax.py
--rw-r--r--   0        0        0     2108 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/mimetypes.py
--rw-r--r--   0        0        0     1741 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/report.py
--rw-r--r--   0        0        0     5336 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/serve.py
--rw-r--r--   0        0        0      235 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/serviceworker.py
--rw-r--r--   0        0        0     4867 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/settings.py
--rw-r--r--   0        0        0     6234 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/static.py
--rw-r--r--   0        0        0     4147 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/translation.py
--rw-r--r--   0        0        0       32 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/tests/__init__.py
--rw-r--r--   0        0        0     2697 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/tests/conftest.py
--rw-r--r--   0        0        0     4591 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/tests/test_archive.py
--rw-r--r--   0        0        0     8350 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/tests/test_cli.py
--rw-r--r--   0        0        0     1516 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/tests/test_cli_aliases_flags.py
--rw-r--r--   0        0        0     2076 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/tests/test_contents.py
--rw-r--r--   0        0        0     2669 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/tests/test_extend_addon.py
--rw-r--r--   0        0        0     2545 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/tests/test_federated.py
--rw-r--r--   0        0        0     1388 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/tests/test_mathjax.py
--rw-r--r--   0        0        0      342 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/tests/test_meta.py
--rw-r--r--   0        0        0     2788 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/tests/test_serve.py
--rw-r--r--   0        0        0    14395 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/jupyterlite_core/tests/fixtures/the-smallest-extension-0.1.0-py_0.conda
--rw-r--r--   0        0        0     2104 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/.gitignore
--rw-r--r--   0        0        0     1524 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/LICENSE
--rw-r--r--   0        0        0     1186 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/README.md
--rw-r--r--   0        0        0     3318 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/pyproject.toml
--rw-r--r--   0        0        0     3729 2023-04-01 06:43:15.000000 jupyterlite_core-0.1.0rc0/PKG-INFO
+-rw-r--r--   0        0        0       67 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/__init__.py
+-rw-r--r--   0        0        0       81 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/__main__.py
+-rw-r--r--   0        0        0    10543 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/app.py
+-rw-r--r--   0        0        0     8940 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/config.py
+-rw-r--r--   0        0        0     4809 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/constants.py
+-rw-r--r--   0        0        0  7436304 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/jupyterlite-app-0.1.1.tgz
+-rw-r--r--   0        0        0     5532 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/manager.py
+-rw-r--r--   0        0        0      691 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/optional.py
+-rw-r--r--   0        0        0      665 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/trait_types.py
+-rw-r--r--   0        0        0     3020 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/addons/__init__.py
+-rw-r--r--   0        0        0     5644 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/addons/archive.py
+-rw-r--r--   0        0        0    13904 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/addons/base.py
+-rw-r--r--   0        0        0     8490 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/addons/contents.py
+-rw-r--r--   0        0        0    11685 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/addons/federated_extensions.py
+-rw-r--r--   0        0        0      153 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/addons/icons.py
+-rw-r--r--   0        0        0     2813 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/addons/lite.py
+-rw-r--r--   0        0        0     4589 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/addons/mathjax.py
+-rw-r--r--   0        0        0     2108 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/addons/mimetypes.py
+-rw-r--r--   0        0        0     1741 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/addons/report.py
+-rw-r--r--   0        0        0     5336 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/addons/serve.py
+-rw-r--r--   0        0        0      235 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/addons/serviceworker.py
+-rw-r--r--   0        0        0     4867 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/addons/settings.py
+-rw-r--r--   0        0        0     6234 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/addons/static.py
+-rw-r--r--   0        0        0     4147 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/addons/translation.py
+-rw-r--r--   0        0        0       32 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/tests/__init__.py
+-rw-r--r--   0        0        0     2697 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/tests/conftest.py
+-rw-r--r--   0        0        0     4591 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/tests/test_archive.py
+-rw-r--r--   0        0        0     8350 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/tests/test_cli.py
+-rw-r--r--   0        0        0     1516 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/tests/test_cli_aliases_flags.py
+-rw-r--r--   0        0        0     3091 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/tests/test_contents.py
+-rw-r--r--   0        0        0     2669 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/tests/test_extend_addon.py
+-rw-r--r--   0        0        0     2545 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/tests/test_federated.py
+-rw-r--r--   0        0        0     1388 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/tests/test_mathjax.py
+-rw-r--r--   0        0        0      342 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/tests/test_meta.py
+-rw-r--r--   0        0        0     2788 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/tests/test_serve.py
+-rw-r--r--   0        0        0    14395 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/jupyterlite_core/tests/fixtures/the-smallest-extension-0.1.0-py_0.conda
+-rw-r--r--   0        0        0     2104 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1524 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1186 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/README.md
+-rw-r--r--   0        0        0     3349 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5483 2023-07-31 13:00:28.000000 jupyterlite_core-0.1.1/PKG-INFO
```

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/app.py` & `jupyterlite_core-0.1.1/jupyterlite_core/app.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/config.py` & `jupyterlite_core-0.1.1/jupyterlite_core/config.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/constants.py` & `jupyterlite_core-0.1.1/jupyterlite_core/constants.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/manager.py` & `jupyterlite_core-0.1.1/jupyterlite_core/manager.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/optional.py` & `jupyterlite_core-0.1.1/jupyterlite_core/optional.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/trait_types.py` & `jupyterlite_core-0.1.1/jupyterlite_core/trait_types.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/__init__.py` & `jupyterlite_core-0.1.1/jupyterlite_core/addons/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/archive.py` & `jupyterlite_core-0.1.1/jupyterlite_core/addons/archive.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/base.py` & `jupyterlite_core-0.1.1/jupyterlite_core/addons/base.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/contents.py` & `jupyterlite_core-0.1.1/jupyterlite_core/addons/contents.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,17 +159,15 @@
 
         self.maybe_timestamp(self.output_files_dir)
 
         from jupyter_server.services.contents.filemanager import FileContentsManager
 
         fm = FileContentsManager(root_dir=str(self.output_files_dir), parent=self)
 
-        listing_path = output_file_dir.as_uri().replace(
-            self.output_files_dir.as_uri(), "/"
-        )
+        listing_path = str(output_file_dir.relative_to(self.output_files_dir))
 
         try:
             listing = fm.get(listing_path)
         except Exception as error:
             print(
                 f"""Couldn't fetch {listing_path} as Jupyter contents.  {error}
                 If this folder, or one of its parents, starts with a `.`, you can
```

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/federated_extensions.py` & `jupyterlite_core-0.1.1/jupyterlite_core/addons/federated_extensions.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/lite.py` & `jupyterlite_core-0.1.1/jupyterlite_core/addons/lite.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/mathjax.py` & `jupyterlite_core-0.1.1/jupyterlite_core/addons/mathjax.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/mimetypes.py` & `jupyterlite_core-0.1.1/jupyterlite_core/addons/mimetypes.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/report.py` & `jupyterlite_core-0.1.1/jupyterlite_core/addons/report.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/serve.py` & `jupyterlite_core-0.1.1/jupyterlite_core/addons/serve.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/settings.py` & `jupyterlite_core-0.1.1/jupyterlite_core/addons/settings.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/static.py` & `jupyterlite_core-0.1.1/jupyterlite_core/addons/static.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/addons/translation.py` & `jupyterlite_core-0.1.1/jupyterlite_core/addons/translation.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/tests/conftest.py` & `jupyterlite_core-0.1.1/jupyterlite_core/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/tests/test_archive.py` & `jupyterlite_core-0.1.1/jupyterlite_core/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/tests/test_cli.py` & `jupyterlite_core-0.1.1/jupyterlite_core/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/tests/test_cli_aliases_flags.py` & `jupyterlite_core-0.1.1/jupyterlite_core/tests/test_cli_aliases_flags.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/tests/test_contents.py` & `jupyterlite_core-0.1.1/jupyterlite_core/tests/test_contents.py`

 * *Files 22% similar despite different names*

```diff
@@ -62,7 +62,40 @@
         hidden_contents = json.loads(hidden_contents_json.read_text(encoding="utf-8"))
 
         postbuild_content = hidden_contents["content"][0]
         assert postbuild_content["name"] == "postBuild", postbuild_content
         assert postbuild_content["path"] == ".binder/postBuild", postbuild_content
     else:
         assert not root_contents_json.exists()
+
+
+def test_contents_with_space(
+    an_empty_lite_dir,
+    script_runner,
+):
+    dir_name = "dir with spaces"
+    contents_dir = an_empty_lite_dir / "contents" / dir_name
+    contents_dir.mkdir(parents=True)
+    file_name = "file name with spaces"
+    contents_file = contents_dir / file_name
+    contents_file.touch()
+
+    result = script_runner.run(
+        "jupyter",
+        "lite",
+        "build",
+        "--contents",
+        "contents",
+        cwd=str(an_empty_lite_dir),
+    )
+    assert result.success
+
+    out = an_empty_lite_dir / "_output"
+    root_contents_json = out / "api/contents/all.json"
+    contents_json = out / f"api/contents/{dir_name}/all.json"
+
+    root_contents = json.loads(root_contents_json.read_text(encoding="utf-8"))
+    assert len(root_contents["content"]) == 1, root_contents
+    contents = json.loads(contents_json.read_text(encoding="utf-8"))
+    content = contents["content"][0]
+    assert content["name"] == file_name
+    assert content["path"] == f"{dir_name}/{file_name}"
```

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/tests/test_extend_addon.py` & `jupyterlite_core-0.1.1/jupyterlite_core/tests/test_extend_addon.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/tests/test_federated.py` & `jupyterlite_core-0.1.1/jupyterlite_core/tests/test_federated.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/tests/test_mathjax.py` & `jupyterlite_core-0.1.1/jupyterlite_core/tests/test_mathjax.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/tests/test_serve.py` & `jupyterlite_core-0.1.1/jupyterlite_core/tests/test_serve.py`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/jupyterlite_core/tests/fixtures/the-smallest-extension-0.1.0-py_0.conda` & `jupyterlite_core-0.1.1/jupyterlite_core/tests/fixtures/the-smallest-extension-0.1.0-py_0.conda`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/.gitignore` & `jupyterlite_core-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/LICENSE` & `jupyterlite_core-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/README.md` & `jupyterlite_core-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlite_core-0.1.0rc0/pyproject.toml` & `jupyterlite_core-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     "js",
     "jupyter",
     "jupyterlab",
     "notebook",
     "pyodide",
     "schema",
 ]
+license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.8"
 dynamic = ["version", "description"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Jupyter",
     "Framework :: Jupyter :: JupyterLab",
```

