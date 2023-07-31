# Comparing `tmp/nipraxis-0.4.tar.gz` & `tmp/nipraxis-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nipraxis-0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "nipraxis-0.4.1.tar", last modified: Mon Jul 31 12:31:56 2023, max compression
```

## Comparing `nipraxis-0.4.tar` & `nipraxis-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       61 2023-07-31 11:58:41.495402 nipraxis-0.4/.coveragerc
--rw-r--r--   0        0        0     1071 2023-07-31 11:58:41.496299 nipraxis-0.4/.github/workflows/testing.yml
--rw-r--r--   0        0        0       65 2023-07-31 11:58:41.497064 nipraxis-0.4/.gitignore
--rw-r--r--   0        0        0     1607 2022-03-18 16:46:56.808775 nipraxis-0.4/LICENSE
--rw-r--r--   0        0        0      278 2023-07-31 12:01:33.420932 nipraxis-0.4/README.md
--rw-r--r--   0        0        0      506 2023-07-31 12:00:44.325251 nipraxis-0.4/nipraxis/__init__.py
--rw-r--r--   0        0        0      249 2023-07-31 11:58:41.498013 nipraxis-0.4/nipraxis/_fetcher.py
--rw-r--r--   0        0        0     1370 2023-07-31 11:58:41.498250 nipraxis-0.4/nipraxis/registry.yaml
--rw-r--r--   0        0        0     1429 2022-04-04 15:15:30.625554 nipraxis-0.4/nipraxis/rotations.py
--rw-r--r--   0        0        0     1424 2022-03-18 16:48:52.342462 nipraxis-0.4/nipraxis/stimuli.py
--rw-r--r--   0        0        0        0 2022-03-18 16:46:56.809485 nipraxis-0.4/nipraxis/tests/__init__.py
--rw-r--r--   0        0        0     1093 2023-07-31 11:58:41.498638 nipraxis-0.4/nipraxis/tests/test_local_cache.py
--rw-r--r--   0        0        0     1087 2022-04-04 15:15:30.625886 nipraxis-0.4/nipraxis/tests/test_rotations.py
--rw-r--r--   0        0        0     1082 2022-03-18 16:51:57.800992 nipraxis-0.4/nipraxis/tests/test_stimuli.py
--rw-r--r--   0        0        0      524 2023-07-31 11:58:41.499076 nipraxis-0.4/pyproject.toml
--rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 nipraxis-0.4/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-07-31 11:58:41.495402 nipraxis-0.4.1/.coveragerc
+-rw-r--r--   0        0        0     1071 2023-07-31 11:58:41.496299 nipraxis-0.4.1/.github/workflows/testing.yml
+-rw-r--r--   0        0        0       65 2023-07-31 11:58:41.497064 nipraxis-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1607 2022-03-18 16:46:56.808775 nipraxis-0.4.1/LICENSE
+-rw-r--r--   0        0        0      278 2023-07-31 12:01:33.420932 nipraxis-0.4.1/README.md
+-rw-r--r--   0        0        0      508 2023-07-31 12:30:05.348489 nipraxis-0.4.1/nipraxis/__init__.py
+-rw-r--r--   0        0        0      220 2023-07-31 12:26:14.871353 nipraxis-0.4.1/nipraxis/_fetcher.py
+-rw-r--r--   0        0        0     1617 2023-07-31 12:29:15.115119 nipraxis-0.4.1/nipraxis/registry.yaml
+-rw-r--r--   0        0        0     1429 2022-04-04 15:15:30.625554 nipraxis-0.4.1/nipraxis/rotations.py
+-rw-r--r--   0        0        0     1424 2022-03-18 16:48:52.342462 nipraxis-0.4.1/nipraxis/stimuli.py
+-rw-r--r--   0        0        0        0 2022-03-18 16:46:56.809485 nipraxis-0.4.1/nipraxis/tests/__init__.py
+-rw-r--r--   0        0        0     1082 2023-07-31 12:25:05.545499 nipraxis-0.4.1/nipraxis/tests/test_local_cache.py
+-rw-r--r--   0        0        0     1087 2022-04-04 15:15:30.625886 nipraxis-0.4.1/nipraxis/tests/test_rotations.py
+-rw-r--r--   0        0        0     1082 2022-03-18 16:51:57.800992 nipraxis-0.4.1/nipraxis/tests/test_stimuli.py
+-rw-r--r--   0        0        0      524 2023-07-31 12:25:05.545789 nipraxis-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 nipraxis-0.4.1/PKG-INFO
```

### Comparing `nipraxis-0.4/.github/workflows/testing.yml` & `nipraxis-0.4.1/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `nipraxis-0.4/LICENSE` & `nipraxis-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nipraxis-0.4/nipraxis/registry.yaml` & `nipraxis-0.4.1/nipraxis/registry.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # Parameters for Pooch data registry
 pkg_name: 'nipraxis'
 base_url: "https://raw.githubusercontent.com/nipraxis/nipraxis-data/{version}/"
 version_dev: "main"
 cache_env_var: "NIPRAXIS_LOCAL_CACHE"
 staging_env_var: "NIPRAXIS_STAGING_CACHE"
-data_version: '0.4'
+data_version: '0.5'
 files:
   'ds107_sub012_highres.nii': 'md5:316b0635a4280f65e1ca27ecb34264d6'
   'ds107_sub012_t1r2.nii': 'md5:4546a0a3f7041261b80b56b60cd54126'
   'ds108_sub001_t1r1.nii': 'md5:6378302aad7bc006bfb48fa973866e68'
   'ds114_sub009_highres.nii': 'md5:95d1b9542a9adebb87e3948c33af478d'
   'ds114_sub009_highres_brain_222.nii': 'md5:615aad84d5b96085601fe306af614564'
   'ds114_sub009_t2r1.nii': 'md5:709fcca8d33ddb7d0b7d501210c8f51c'
+  'ds114_sub009_highres_brain_mask.nii': 'md5:3f5d42c8220f1f65e5d62f7eed6f7ef3'
+  'mni_icbm152_t1_tal_nlin_asym_09a.nii': 'md5:1ea8f4f1e41bc17a94602e48141fdbc8'
+  'mni_icbm152_t1_tal_nlin_asym_09a_mask.nii': 'md5:250bcb6ea9d20242e5d18736cb2793fd'
   'mni_icbm152_t1_tal_nlin_asym_09a_masked_222.nii': 'md5:6d0615d6581c9f9e17f6916da480fd2e'
   'camera.txt': 'md5:e596928a61c4332252d4eb1f0b6dab1e'
   'ds114_sub009_highres_moved.hdr': 'md5:b12b3d9db549d68b984ace0b95920603'
   'ds114_sub009_highres_moved.img': 'md5:95d1b9542a9adebb87e3948c33af478d'
   'ds114_sub009_t2r1_cond.txt': 'md5:5cb29aed9c9f330afe1af7e69f8aad18'
   'new_cond.txt': 'md5:b40dc95801267932a9f273f02ac05d1e'
   'ds114_sub009_t2r1_conv.txt': 'md5:839eadd4533af9d8aef0cf8d623ab139'
```

### Comparing `nipraxis-0.4/nipraxis/rotations.py` & `nipraxis-0.4.1/nipraxis/rotations.py`

 * *Files identical despite different names*

### Comparing `nipraxis-0.4/nipraxis/stimuli.py` & `nipraxis-0.4.1/nipraxis/stimuli.py`

 * *Files identical despite different names*

### Comparing `nipraxis-0.4/nipraxis/tests/test_local_cache.py` & `nipraxis-0.4.1/nipraxis/tests/test_local_cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 def test_camera(tmp_path, monkeypatch):
     local_cache = tmp_path / 'nipraxis-local'
     staging_cache = tmp_path / 'nipraxis-staging'
     monkeypatch.delenv("NIPRAXIS_STAGING_CACHE", raising=False)
     monkeypatch.setenv("NIPRAXIS_LOCAL_CACHE", str(local_cache))
     fetcher = unscrewed.Fetcher(npxf._config_file)
-    monkeypatch.setattr('nipraxis._fetcher.fetch_file', fetcher.fetch_file)
+    monkeypatch.setattr('nipraxis._fetcher.fetch_file', fetcher)
     fname = npxf.fetch_file('camera.txt')
     assert fname.startswith(str(local_cache))
     monkeypatch.setenv("NIPRAXIS_STAGING_CACHE", str(staging_cache))
     fname = npxf.fetch_file('camera.txt')
     assert fname.startswith(str(local_cache))
     shutil.move(local_cache, staging_cache)
     fname = npxf.fetch_file('camera.txt')
```

### Comparing `nipraxis-0.4/nipraxis/tests/test_rotations.py` & `nipraxis-0.4.1/nipraxis/tests/test_rotations.py`

 * *Files identical despite different names*

### Comparing `nipraxis-0.4/nipraxis/tests/test_stimuli.py` & `nipraxis-0.4.1/nipraxis/tests/test_stimuli.py`

 * *Files identical despite different names*

### Comparing `nipraxis-0.4/pyproject.toml` & `nipraxis-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nipraxis-0.4/PKG-INFO` & `nipraxis-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nipraxis
-Version: 0.4
+Version: 0.4.1
 Summary: Nipraxis utilities
 Author-email: The Nipraxis team <matthew.brett@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: numpy
 Requires-Dist: unscrewed
```

