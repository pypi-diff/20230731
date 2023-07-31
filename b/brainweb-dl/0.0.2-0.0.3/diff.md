# Comparing `tmp/brainweb-dl-0.0.2.tar.gz` & `tmp/brainweb-dl-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainweb-dl-0.0.2.tar", last modified: Sat Jul 22 20:58:09 2023, max compression
+gzip compressed data, was "brainweb-dl-0.0.3.tar", last modified: Mon Jul 31 20:22:17 2023, max compression
```

## Comparing `brainweb-dl-0.0.2.tar` & `brainweb-dl-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:58:09.601989 brainweb-dl-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:58:09.593989 brainweb-dl-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:58:09.597989 brainweb-dl-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-22 20:57:39.000000 brainweb-dl-0.0.2/.github/workflows/master-cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-22 20:57:39.000000 brainweb-dl-0.0.2/.github/workflows/tags-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-22 20:57:39.000000 brainweb-dl-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-22 20:58:09.601989 brainweb-dl-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-07-22 20:57:39.000000 brainweb-dl-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-22 20:57:39.000000 brainweb-dl-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 20:58:09.601989 brainweb-dl-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:58:09.593989 brainweb-dl-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:58:09.597989 brainweb-dl-0.0.2/src/brainweb_dl/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-22 20:57:39.000000 brainweb-dl-0.0.2/src/brainweb_dl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13839 2023-07-22 20:57:39.000000 brainweb-dl-0.0.2/src/brainweb_dl/_brainweb.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-22 20:58:09.000000 brainweb-dl-0.0.2/src/brainweb_dl/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-22 20:57:39.000000 brainweb-dl-0.0.2/src/brainweb_dl/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:58:09.597989 brainweb-dl-0.0.2/src/brainweb_dl/data/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-22 20:57:39.000000 brainweb-dl-0.0.2/src/brainweb_dl/data/brainweb1_tissues.csv
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-22 20:57:39.000000 brainweb-dl-0.0.2/src/brainweb_dl/data/brainweb20_tissues.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-22 20:57:39.000000 brainweb-dl-0.0.2/src/brainweb_dl/mri.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:58:09.597989 brainweb-dl-0.0.2/src/brainweb_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-22 20:58:09.000000 brainweb-dl-0.0.2/src/brainweb_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-22 20:58:09.000000 brainweb-dl-0.0.2/src/brainweb_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 20:58:09.000000 brainweb-dl-0.0.2/src/brainweb_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-22 20:58:09.000000 brainweb-dl-0.0.2/src/brainweb_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-22 20:58:09.000000 brainweb-dl-0.0.2/src/brainweb_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-22 20:58:09.000000 brainweb-dl-0.0.2/src/brainweb_dl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 20:58:09.601989 brainweb-dl-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-22 20:57:39.000000 brainweb-dl-0.0.2/tests/test_brainweb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:22:17.081107 brainweb-dl-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:22:17.081107 brainweb-dl-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:22:17.081107 brainweb-dl-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-31 20:21:43.000000 brainweb-dl-0.0.3/.github/workflows/master-cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-31 20:21:43.000000 brainweb-dl-0.0.3/.github/workflows/tags-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-31 20:21:43.000000 brainweb-dl-0.0.3/.github/workflows/test-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-31 20:21:43.000000 brainweb-dl-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-31 20:21:43.000000 brainweb-dl-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-07-31 20:22:17.081107 brainweb-dl-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-31 20:21:43.000000 brainweb-dl-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-31 20:21:43.000000 brainweb-dl-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 20:22:17.085108 brainweb-dl-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:22:17.081107 brainweb-dl-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:22:17.081107 brainweb-dl-0.0.3/src/brainweb_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-31 20:21:43.000000 brainweb-dl-0.0.3/src/brainweb_dl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-07-31 20:21:43.000000 brainweb-dl-0.0.3/src/brainweb_dl/_brainweb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-31 20:22:16.000000 brainweb-dl-0.0.3/src/brainweb_dl/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-31 20:21:43.000000 brainweb-dl-0.0.3/src/brainweb_dl/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:22:17.081107 brainweb-dl-0.0.3/src/brainweb_dl/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-31 20:21:43.000000 brainweb-dl-0.0.3/src/brainweb_dl/data/brainweb1_tissues.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-31 20:21:43.000000 brainweb-dl-0.0.3/src/brainweb_dl/data/brainweb20_tissues.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-07-31 20:21:43.000000 brainweb-dl-0.0.3/src/brainweb_dl/mri.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:22:17.081107 brainweb-dl-0.0.3/src/brainweb_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-07-31 20:22:17.000000 brainweb-dl-0.0.3/src/brainweb_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-31 20:22:17.000000 brainweb-dl-0.0.3/src/brainweb_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 20:22:17.000000 brainweb-dl-0.0.3/src/brainweb_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-31 20:22:17.000000 brainweb-dl-0.0.3/src/brainweb_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-31 20:22:17.000000 brainweb-dl-0.0.3/src/brainweb_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 20:22:17.000000 brainweb-dl-0.0.3/src/brainweb_dl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:22:17.081107 brainweb-dl-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-31 20:21:43.000000 brainweb-dl-0.0.3/tests/test_brainweb.py
```

### Comparing `brainweb-dl-0.0.2/.github/workflows/master-cd.yml` & `brainweb-dl-0.0.3/.github/workflows/master-cd.yml`

 * *Files identical despite different names*

### Comparing `brainweb-dl-0.0.2/.github/workflows/tags-release.yml` & `brainweb-dl-0.0.3/.github/workflows/tags-release.yml`

 * *Files identical despite different names*

### Comparing `brainweb-dl-0.0.2/LICENSE` & `brainweb-dl-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `brainweb-dl-0.0.2/PKG-INFO` & `brainweb-dl-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainweb-dl
-Version: 0.0.2
+Version: 0.0.3
 Summary: Download BrainWeb MRI data
 Author-email: Pierre-Antoine Comby <pierre-antoine.comby@cea.fr>
 License: MIT License
         
         Copyright (c) 2023 Pierre-Antoine Comby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,14 +50,15 @@
 Welcome to Brainweb-DL, a powerful Python toolkit for downloading and converting the Brainweb dataset. 
 
 <p align="center">
 <a href=https://github.com/paquiteau/brainweb-dl/blob/master/LICENSE><img src=https://img.shields.io/github/license/paquiteau/brainweb-dl></a>
 <a href=https://www.codefactor.io/repository/github/paquiteau/brainweb-dl><img src=https://www.codefactor.io/repository/github/paquiteau/brainweb-dl/badge></a>
 <a href=https://github.com/psf/black><img src=https://img.shields.io/badge/style-black-black></a>
 <a href=https://pypi.org/project/brainweb-dl><img src=https://img.shields.io/pypi/v/brainweb-dl></a>
+<a href=https://pypi.org/project/brainweb-dl><img src=https://img.shields.io/pypi/pyversions/brainweb-dl></a>
 </p>
 
 ## Features
 
 - **Effortless Dataset Management:** Automatically download, cache, and format the Brainweb dataset with ease. Convert it to the convenient nifti format or numpy array hassle-free.
 
 - **Multiple Image Generation:** Generate high-quality T1, T2, T2*, and PD images directly from the Brainweb dataset. Perfect for testing purposes, although keep in mind that the values provided are approximate.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: brainweb-dl Version: 0.0.2 Summary: Download
+Metadata-Version: 2.1 Name: brainweb-dl Version: 0.0.3 Summary: Download
 BrainWeb MRI data Author-email: Pierre-Antoine Comby
 comby@cea.fr> License: MIT License Copyright (c) 2023 Pierre-Antoine Comby
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
@@ -26,15 +26,15 @@
 Python :: 3.11 Requires-Python: >=3.6 Description-Content-Type: text/markdown
 Provides-Extra: dev Provides-Extra: test Provides-Extra: doc License-File:
 LICENSE # Brainweb-DL Welcome to Brainweb-DL, a powerful Python toolkit for
 downloading and converting the Brainweb dataset.
     [https://img.shields.io/github/license/paquiteau/brainweb-dl] [https://
   www.codefactor.io/repository/github/paquiteau/brainweb-dl/badge] [https://
     img.shields.io/badge/style-black-black] [https://img.shields.io/pypi/v/
-                                 brainweb-dl]
+       brainweb-dl] [https://img.shields.io/pypi/pyversions/brainweb-dl]
 ## Features - **Effortless Dataset Management:** Automatically download, cache,
 and format the Brainweb dataset with ease. Convert it to the convenient nifti
 format or numpy array hassle-free. - **Multiple Image Generation:** Generate
 high-quality T1, T2, T2*, and PD images directly from the Brainweb dataset.
 Perfect for testing purposes, although keep in mind that the values provided
 are approximate. ### Available data The Brainweb project kindly provides: - A
 normal brain phantom (named subject `0` afterwards), with T1, T2 and PD
```

### Comparing `brainweb-dl-0.0.2/README.md` & `brainweb-dl-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Welcome to Brainweb-DL, a powerful Python toolkit for downloading and converting the Brainweb dataset. 
 
 <p align="center">
 <a href=https://github.com/paquiteau/brainweb-dl/blob/master/LICENSE><img src=https://img.shields.io/github/license/paquiteau/brainweb-dl></a>
 <a href=https://www.codefactor.io/repository/github/paquiteau/brainweb-dl><img src=https://www.codefactor.io/repository/github/paquiteau/brainweb-dl/badge></a>
 <a href=https://github.com/psf/black><img src=https://img.shields.io/badge/style-black-black></a>
 <a href=https://pypi.org/project/brainweb-dl><img src=https://img.shields.io/pypi/v/brainweb-dl></a>
+<a href=https://pypi.org/project/brainweb-dl><img src=https://img.shields.io/pypi/pyversions/brainweb-dl></a>
 </p>
 
 ## Features
 
 - **Effortless Dataset Management:** Automatically download, cache, and format the Brainweb dataset with ease. Convert it to the convenient nifti format or numpy array hassle-free.
 
 - **Multiple Image Generation:** Generate high-quality T1, T2, T2*, and PD images directly from the Brainweb dataset. Perfect for testing purposes, although keep in mind that the values provided are approximate.
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # Brainweb-DL Welcome to Brainweb-DL, a powerful Python toolkit for downloading
 and converting the Brainweb dataset.
     [https://img.shields.io/github/license/paquiteau/brainweb-dl] [https://
   www.codefactor.io/repository/github/paquiteau/brainweb-dl/badge] [https://
     img.shields.io/badge/style-black-black] [https://img.shields.io/pypi/v/
-                                 brainweb-dl]
+       brainweb-dl] [https://img.shields.io/pypi/pyversions/brainweb-dl]
 ## Features - **Effortless Dataset Management:** Automatically download, cache,
 and format the Brainweb dataset with ease. Convert it to the convenient nifti
 format or numpy array hassle-free. - **Multiple Image Generation:** Generate
 high-quality T1, T2, T2*, and PD images directly from the Brainweb dataset.
 Perfect for testing purposes, although keep in mind that the values provided
 are approximate. ### Available data The Brainweb project kindly provides: - A
 normal brain phantom (named subject `0` afterwards), with T1, T2 and PD
```

### Comparing `brainweb-dl-0.0.2/pyproject.toml` & `brainweb-dl-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `brainweb-dl-0.0.2/src/brainweb_dl/__init__.py` & `brainweb-dl-0.0.3/src/brainweb_dl/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Brainweb downloader."""
 from .mri import get_mri
 
 from ._brainweb import (
     get_brainweb1_seg,
     get_brainweb1,
     get_brainweb20,
     get_brainweb20_multiple,
```

### Comparing `brainweb-dl-0.0.2/src/brainweb_dl/_brainweb.py` & `brainweb-dl-0.0.3/src/brainweb_dl/_brainweb.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     - The environment variable BRAINWEB_DIR.
     - The defaultbrainweb_directory ~/.cache/brainweb.
     """
     if brainweb_dir is None:
         brainweb_dir = os.environ.get("BRAINWEB_DIR", None)
     if brainweb_dir is None:
         brainweb_dir = Path.home() / ".cache" / "brainweb"
-    os.makedirs(brainweb_dir, exist_ok=True)
+    os.makedirs(Path(brainweb_dir), exist_ok=True)
     return Path(brainweb_dir)
 
 
 def get_brainweb20_multiple(
     subject: int | list | Literal["all"],
     brainweb_dir: os.PathLike = None,
     force: bool = False,
@@ -295,17 +295,15 @@
 def get_brainweb1_seg(
     segmentation: Literal["crisp", "fuzzy"] = "crisp",
     extension: Literal["nii.gz", "nii"] = "nii.gz",
     brainweb_dir: os.PathLike = ".brainweb",
     force: bool = False,
 ) -> os.PathLike:
     """Download the Brainweb1 phantom segmentation as a nifti file."""
-    # The case of fuzzy segmentation is a bit special.
-    # We download all the fuzzy segmentation and create a 4D volume.
-    # The 4th dimension is the segmentation type.
+    brainweb_dir = get_brainweb_dir(brainweb_dir)
     if segmentation not in ["crisp", "fuzzy"]:
         raise ValueError("type must be in {'crisp', 'fuzzy'}")
     if segmentation == "crisp":
         download_command = "phantom_1.0mm_normal_crisp"
         fname = f"phantom_1.0mm_normal_crisp.{extension}"
         path = brainweb_dir / fname
         if path.exists() and not force:
@@ -313,21 +311,20 @@
         return _request_get_brainweb(
             download_command,
             brainweb_dir / fname,
             force,
             shape=STD_RES,
             dtype=np.uint16,
         )
-    brainweb_dir = get_brainweb_dir(brainweb_dir)
     fname = f"phantom_1.0mm_normal_fuzzy.{extension}"
     path = brainweb_dir / fname
     if path.exists() and not force:
         return path
     tissue_map = _load_tissue_map(1)
-    data = np.zeros((*STD_RES, len(tissue_map)))
+    data = np.zeros((*STD_RES, len(tissue_map)), dtype=np.uint16)
     for i, row in tqdm(
         enumerate(tissue_map),
         desc="Downloading tissues",
         total=len(tissue_map),
         position=1,
         leave=False,
     ):
@@ -336,15 +333,15 @@
             name,
             path=brainweb_dir / f"{name}.{extension}",  # placeholder
             dtype=np.uint16,
             shape=STD_RES,
             obj_mode=True,
         )
     # Create the 4D volume.
-    nib.save(nib.Nifti1Image(data, affine=np.eye(4)), path)
+    nib.save(nib.Nifti1Image(abs(data), affine=np.eye(4)), path)
     return path
 
 
 def _request_get_brainweb(
     download_command: str,
     path: os.PathLike,
     force: bool = False,
@@ -419,15 +416,15 @@
         for chunk in d.iter_content(chunk_size=1024):
             if chunk:
                 buffer.write(chunk)
                 pbar.update(len(chunk))
         data = np.frombuffer(gzip.decompress(buffer.getvalue()), dtype=dtype)
     if data.size != np.prod(shape):
         raise ValueError(f"Mismatch between data size and shape {data.size} != {shape}")
-    data = data.reshape(shape)
+    data = abs(data).reshape(shape)
     if obj_mode:
         return data
 
     return save_array(data, path)
 
 
 @functools.lru_cache(maxsize=3)
```

### Comparing `brainweb-dl-0.0.2/src/brainweb_dl/cli.py` & `brainweb-dl-0.0.3/src/brainweb_dl/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """CLI function for the package."""
 from __future__ import annotations
 import argparse
-import logging
 
 import nibabel as nib
 import numpy as np
 
-from ._brainweb import SUB_ID, get_brainweb1, get_brainweb1_seg, get_brainweb20_multiple
+from ._brainweb import SUB_ID, get_brainweb1_seg, get_brainweb20_multiple
 from .mri import get_mri
 
 
 def parse_args() -> argparse.Namespace:
     """Parse command-line arguments."""
     parser = argparse.ArgumentParser(
         description="Get data from the brainWeb Dataset",
```

### Comparing `brainweb-dl-0.0.2/src/brainweb_dl/mri.py` & `brainweb-dl-0.0.3/src/brainweb_dl/mri.py`

 * *Files 12% similar despite different names*

```diff
@@ -60,46 +60,79 @@
 
     Returns
     -------
     np.ndarray
         MRI data.
     """
     if sub_id == 0:
-        if contrast != "T2*":
+        if contrast in ["T1", "T2", "PD"]:
             filename = get_brainweb1(
                 contrast,
                 res=res,
                 noise=noise,
                 field_value=field_value,
                 brainweb_dir=brainweb_dir,
                 force=force,
             )
-            data = nib.load(filename).get_fdata()
-            return data
 
-        logger.warning(
-            "Brainweb 1 does not have T2* data. The values are going to be empirical."
-        )
-        filename = get_brainweb1_seg(
-            "fuzzy",
-            force=force,
-            brainweb_dir=brainweb_dir,
-        )
-
-        return _apply_contrast(filename, 1, contrast, rng)
-    if contrast == "T1":
-        filename = get_brainweb20_T1(sub_id)
-        data = nib.load(filename).get_fdata()
+            data = nib.load(filename)
+            data = data.get_fdata()
+
+        elif contrast == "T2*":
+            logger.warning(
+                "Brainweb 1 does not have T2* data. The provided values are empirical."
+            )
+            filename = get_brainweb1_seg(
+                "fuzzy",
+                force=force,
+                brainweb_dir=brainweb_dir,
+            )
+
+            data = _apply_contrast(filename, 1, contrast, rng)
+        elif contrast in ["fuzzy", "crisp"]:
+            filename = get_brainweb1_seg(
+                contrast, force=force, brainweb_dir=brainweb_dir
+            )
+            data = nib.load(filename)
+            data = np.asanyarray(data.dataobj, dtype=np.uint16)
+            if contrast == "fuzzy":
+                data = data.astype(np.float32) / 4095
+        else:
+            raise ValueError(f"Unknown contrast {contrast}")
     else:
-        filename = get_brainweb20(sub_id, segmentation="fuzzy")
-        data = _apply_contrast(filename, 20, contrast, rng)
+        if contrast == "T1":
+            filename = get_brainweb20_T1(sub_id)
+            data = nib.load(filename).get_fdata()
+        else:
+            filename = get_brainweb20(sub_id, segmentation="fuzzy")
+            data = _apply_contrast(filename, 20, contrast, rng)
 
     if shape is not None and shape != data.shape:
+        if isinstance(shape, float):
+            zoom = shape
+            zoom = (zoom,) * 3
+        elif -1 in shape:
+            if np.prod(data.shape) <= 0:
+                raise ValueError(
+                    "The zoom factor should only have two -1 in its definition"
+                    "(ex. `(-1,-1, 64)` )."
+                )
+            ref_ax = [i for i, v in enumerate(shape) if v > 0][0]
+            zoom = shape[ref_ax] / data.shape[ref_ax]
+            zoom = (zoom,) * 3
+        else:
+            zoom = np.array(shape) / np.array(data.shape)
+
+        if contrast == "fuzzy":
+            # Don't rescale the tissue dimension.
+            zoom = (*zoom, 1)
         # rescale the data
-        data_rescaled = sp.ndimage.zoom(data, np.array(shape) / np.array(data.shape))
+        data_rescaled = sp.ndimage.zoom(data, zoom=zoom)
+        # clip the data to the original range.
+        data_rescaled = np.clip(data_rescaled, data.min(), data.max())
         return data_rescaled
     else:
         return data
 
 
 def _apply_contrast(
     file_fuzzy: os.PathLike,
@@ -118,20 +151,20 @@
     rng : int | np.random.Generator
         Random number generator.
 
     Returns
     -------
     np.ndarray
         MRI data with the applied contrast.
-
     """
     rng = np.random.default_rng(rng)
 
     tissues = _load_tissue_map(tissue_map)
     data = nib.load(file_fuzzy).get_fdata(dtype=np.float32)
+    data /= 4095  # Data was encode in 12 bits
     ret_data = np.zeros(data.shape[:-1], dtype=np.float32)
     contrast_mean = []
     contrast_std = []
     for t in tissues:
         contrast_mean.append(float(t[f"{contrast} (ms)"]))
         try:
             std_val = float(t[f"{contrast} Std (ms)"])
```

### Comparing `brainweb-dl-0.0.2/src/brainweb_dl.egg-info/PKG-INFO` & `brainweb-dl-0.0.3/src/brainweb_dl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainweb-dl
-Version: 0.0.2
+Version: 0.0.3
 Summary: Download BrainWeb MRI data
 Author-email: Pierre-Antoine Comby <pierre-antoine.comby@cea.fr>
 License: MIT License
         
         Copyright (c) 2023 Pierre-Antoine Comby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,14 +50,15 @@
 Welcome to Brainweb-DL, a powerful Python toolkit for downloading and converting the Brainweb dataset. 
 
 <p align="center">
 <a href=https://github.com/paquiteau/brainweb-dl/blob/master/LICENSE><img src=https://img.shields.io/github/license/paquiteau/brainweb-dl></a>
 <a href=https://www.codefactor.io/repository/github/paquiteau/brainweb-dl><img src=https://www.codefactor.io/repository/github/paquiteau/brainweb-dl/badge></a>
 <a href=https://github.com/psf/black><img src=https://img.shields.io/badge/style-black-black></a>
 <a href=https://pypi.org/project/brainweb-dl><img src=https://img.shields.io/pypi/v/brainweb-dl></a>
+<a href=https://pypi.org/project/brainweb-dl><img src=https://img.shields.io/pypi/pyversions/brainweb-dl></a>
 </p>
 
 ## Features
 
 - **Effortless Dataset Management:** Automatically download, cache, and format the Brainweb dataset with ease. Convert it to the convenient nifti format or numpy array hassle-free.
 
 - **Multiple Image Generation:** Generate high-quality T1, T2, T2*, and PD images directly from the Brainweb dataset. Perfect for testing purposes, although keep in mind that the values provided are approximate.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: brainweb-dl Version: 0.0.2 Summary: Download
+Metadata-Version: 2.1 Name: brainweb-dl Version: 0.0.3 Summary: Download
 BrainWeb MRI data Author-email: Pierre-Antoine Comby
 comby@cea.fr> License: MIT License Copyright (c) 2023 Pierre-Antoine Comby
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
@@ -26,15 +26,15 @@
 Python :: 3.11 Requires-Python: >=3.6 Description-Content-Type: text/markdown
 Provides-Extra: dev Provides-Extra: test Provides-Extra: doc License-File:
 LICENSE # Brainweb-DL Welcome to Brainweb-DL, a powerful Python toolkit for
 downloading and converting the Brainweb dataset.
     [https://img.shields.io/github/license/paquiteau/brainweb-dl] [https://
   www.codefactor.io/repository/github/paquiteau/brainweb-dl/badge] [https://
     img.shields.io/badge/style-black-black] [https://img.shields.io/pypi/v/
-                                 brainweb-dl]
+       brainweb-dl] [https://img.shields.io/pypi/pyversions/brainweb-dl]
 ## Features - **Effortless Dataset Management:** Automatically download, cache,
 and format the Brainweb dataset with ease. Convert it to the convenient nifti
 format or numpy array hassle-free. - **Multiple Image Generation:** Generate
 high-quality T1, T2, T2*, and PD images directly from the Brainweb dataset.
 Perfect for testing purposes, although keep in mind that the values provided
 are approximate. ### Available data The Brainweb project kindly provides: - A
 normal brain phantom (named subject `0` afterwards), with T1, T2 and PD
```

### Comparing `brainweb-dl-0.0.2/src/brainweb_dl.egg-info/SOURCES.txt` & `brainweb-dl-0.0.3/src/brainweb_dl.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+.gitignore
 LICENSE
 README.md
 pyproject.toml
 .github/workflows/master-cd.yml
 .github/workflows/tags-release.yml
+.github/workflows/test-ci.yml
 src/brainweb_dl/__init__.py
 src/brainweb_dl/_brainweb.py
 src/brainweb_dl/_version.py
 src/brainweb_dl/cli.py
 src/brainweb_dl/mri.py
 src/brainweb_dl.egg-info/PKG-INFO
 src/brainweb_dl.egg-info/SOURCES.txt
```

### Comparing `brainweb-dl-0.0.2/tests/test_brainweb.py` & `brainweb-dl-0.0.3/tests/test_brainweb.py`

 * *Files identical despite different names*

