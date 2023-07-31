# Comparing `tmp/wandb-core-alpha-0.0.1a1.tar.gz` & `tmp/wandb-core-alpha-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wandb-core-alpha-0.0.1a1.tar", last modified: Tue Jun 27 00:18:33 2023, max compression
+gzip compressed data, was "wandb-core-alpha-0.0.1a2.tar", last modified: Mon Jul 31 12:40:56 2023, max compression
```

## Comparing `wandb-core-alpha-0.0.1a1.tar` & `wandb-core-alpha-0.0.1a2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-06-27 00:18:33.672528 wandb-core-alpha-0.0.1a1/
--rw-r--r--   0 jeff       (501) staff       (20)       58 2023-05-27 20:16:41.000000 wandb-core-alpha-0.0.1a1/MANIFEST.in
--rw-r--r--   0 jeff       (501) staff       (20)      126 2023-06-27 00:18:33.672364 wandb-core-alpha-0.0.1a1/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)       38 2023-06-27 00:18:33.672588 wandb-core-alpha-0.0.1a1/setup.cfg
--rw-r--r--   0 jeff       (501) staff       (20)     3817 2023-06-27 00:18:01.000000 wandb-core-alpha-0.0.1a1/setup.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-06-27 00:18:33.671204 wandb-core-alpha-0.0.1a1/wandb_core/
--rw-r--r--   0 jeff       (501) staff       (20)      308 2023-06-25 04:14:51.000000 wandb-core-alpha-0.0.1a1/wandb_core/__init__.py
-drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-06-27 00:18:33.672106 wandb-core-alpha-0.0.1a1/wandb_core_alpha.egg-info/
--rw-r--r--   0 jeff       (501) staff       (20)      126 2023-06-27 00:18:33.000000 wandb-core-alpha-0.0.1a1/wandb_core_alpha.egg-info/PKG-INFO
--rw-r--r--   0 jeff       (501) staff       (20)      242 2023-06-27 00:18:33.000000 wandb-core-alpha-0.0.1a1/wandb_core_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 jeff       (501) staff       (20)        1 2023-06-27 00:18:33.000000 wandb-core-alpha-0.0.1a1/wandb_core_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 jeff       (501) staff       (20)        1 2023-06-27 00:18:33.000000 wandb-core-alpha-0.0.1a1/wandb_core_alpha.egg-info/not-zip-safe
--rw-r--r--   0 jeff       (501) staff       (20)       11 2023-06-27 00:18:33.000000 wandb-core-alpha-0.0.1a1/wandb_core_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-31 12:40:56.158354 wandb-core-alpha-0.0.1a2/
+-rw-r--r--   0 jeff       (501) staff       (20)       58 2023-07-18 10:51:23.000000 wandb-core-alpha-0.0.1a2/MANIFEST.in
+-rw-r--r--   0 jeff       (501) staff       (20)      126 2023-07-31 12:40:56.158208 wandb-core-alpha-0.0.1a2/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)        0 2023-07-21 14:16:15.000000 wandb-core-alpha-0.0.1a2/pyproject.toml
+-rw-r--r--   0 jeff       (501) staff       (20)       38 2023-07-31 12:40:56.158402 wandb-core-alpha-0.0.1a2/setup.cfg
+-rw-r--r--   0 jeff       (501) staff       (20)     4095 2023-07-31 12:36:47.000000 wandb-core-alpha-0.0.1a2/setup.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-31 12:40:56.157244 wandb-core-alpha-0.0.1a2/wandb_core/
+-rw-r--r--   0 jeff       (501) staff       (20)      308 2023-07-18 10:51:23.000000 wandb-core-alpha-0.0.1a2/wandb_core/__init__.py
+drwxr-xr-x   0 jeff       (501) staff       (20)        0 2023-07-31 12:40:56.157991 wandb-core-alpha-0.0.1a2/wandb_core_alpha.egg-info/
+-rw-r--r--   0 jeff       (501) staff       (20)      126 2023-07-31 12:40:56.000000 wandb-core-alpha-0.0.1a2/wandb_core_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 jeff       (501) staff       (20)      257 2023-07-31 12:40:56.000000 wandb-core-alpha-0.0.1a2/wandb_core_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        1 2023-07-31 12:40:56.000000 wandb-core-alpha-0.0.1a2/wandb_core_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff       (501) staff       (20)        1 2023-07-31 12:40:56.000000 wandb-core-alpha-0.0.1a2/wandb_core_alpha.egg-info/not-zip-safe
+-rw-r--r--   0 jeff       (501) staff       (20)       11 2023-07-31 12:40:56.000000 wandb-core-alpha-0.0.1a2/wandb_core_alpha.egg-info/top_level.txt
```

### Comparing `wandb-core-alpha-0.0.1a1/setup.py` & `wandb-core-alpha-0.0.1a2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,23 @@
         env = {}
         if goos:
             env["GOOS"] = goos
         if goarch:
             env["GOARCH"] = goarch
         env["CGO_ENABLED"] = "0"
         os.makedirs(nexus_path.parent, exist_ok=True)
-        ldflags = "-s -w"
+
+        # Sentry only allows 12 characters for release names, the full commit hash won't fit
+        commit = (
+            subprocess.check_output(["git", "rev-parse", "HEAD"], cwd=src_dir)
+            .decode("utf-8")
+            .strip()
+        )
+
+        ldflags = f"-s -w -X main.commit={commit}"
         cmd = (
             "go",
             "build",
             f"-ldflags={ldflags}",
             "-o",
             str(nexus_path),
             "cmd/nexus/main.go",
@@ -118,15 +126,15 @@
 
     def run(self):
         bdist_wheel.run(self)
 
 
 setup(
     name="wandb-core" if not _is_wandb_core_alpha else "wandb-core-alpha",
-    version="0.0.1a1",
+    version="0.0.1a2",
     description="Wandb core",
     packages=[PACKAGE],
     zip_safe=False,
     include_package_data=True,
     license="MIT license",
     python_requires=">=3.6",
     cmdclass={
```

