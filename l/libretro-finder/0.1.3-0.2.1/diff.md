# Comparing `tmp/libretro_finder-0.1.3.tar.gz` & `tmp/libretro_finder-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretro_finder-0.1.3.tar", max compression
+gzip compressed data, was "libretro_finder-0.2.1.tar", max compression
```

## Comparing `libretro_finder-0.1.3.tar` & `libretro_finder-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1760 2023-07-25 13:44:19.751110 libretro_finder-0.1.3/config/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 13:44:19.751110 libretro_finder-0.1.3/libretro_finder/__init__.py
--rw-r--r--   0        0        0     3667 2023-07-25 13:44:19.751110 libretro_finder-0.1.3/libretro_finder/main.py
--rw-r--r--   0        0        0     1716 2023-07-25 13:44:19.751110 libretro_finder-0.1.3/libretro_finder/utils.py
--rw-r--r--   0        0        0    35823 2023-03-22 16:43:29.653449 libretro_finder-0.1.3/LICENSE
--rw-r--r--   0        0        0      869 2023-07-25 20:12:16.218912 libretro_finder-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3931 2023-07-25 19:12:24.999840 libretro_finder-0.1.3/README.md
--rw-r--r--   0        0        0     4672 1970-01-01 00:00:00.000000 libretro_finder-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2098 2023-07-31 21:55:12.526686 libretro_finder-0.2.1/config/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 13:44:19.751110 libretro_finder-0.2.1/libretro_finder/__init__.py
+-rw-r--r--   0        0        0     4160 2023-07-31 21:55:12.526686 libretro_finder-0.2.1/libretro_finder/main.py
+-rw-r--r--   0        0        0     5979 2023-07-31 21:55:12.527685 libretro_finder-0.2.1/libretro_finder/utils.py
+-rw-r--r--   0        0        0    35823 2023-03-22 16:43:29.653449 libretro_finder-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1033 2023-07-31 21:55:12.527685 libretro_finder-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5539 2023-07-31 21:55:12.525685 libretro_finder-0.2.1/README.md
+-rw-r--r--   0        0        0     6396 1970-01-01 00:00:00.000000 libretro_finder-0.2.1/PKG-INFO
```

### Comparing `libretro_finder-0.1.3/config/__init__.py` & `libretro_finder-0.2.1/config/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
+import sys
 import pathlib
 import re
 import urllib.request
 
 import pandas as pd
+from libretro_finder.utils import find_retroarch
 
-# not expecting BIOS files over 15mb
-MAX_BIOS_BYTES = 15728640
 SEED = 0
 
 # Pulling all BIOS names and hashes from Libretro's system.dat (https://docs.libretro.com/)
 FILE_PATH = pathlib.Path(__file__).parent / "system.dat"
 GITHUB_URL = (
     "https://raw.githubusercontent.com/libretro/libretro-database/master/dat/System.dat"
 )
 if not FILE_PATH.exists():
     print("Getting BIOS names from libretro-database..")
     urllib.request.urlretrieve(GITHUB_URL, FILE_PATH)
     print("Done.")
 
 # Parsing Libretro's system.dat and formatting as pandas dataframe
-index = 0 # pylint: disable=invalid-name
+index = 0  # pylint: disable=invalid-name
 SYSTEMS = []
-with open(FILE_PATH, "r", encoding='utf-8') as file:
+with open(FILE_PATH, "r", encoding="utf-8") as file:
     for line in file:
         line = line.strip()
         if line.startswith("comment"):
             current_system = line.split('"')[1]
         elif line.startswith("rom"):
             match = re.search(
                 r"name (\S+)(?: size (\S+))?(?: crc (\S+))?(?: md5 (\S+))?(?: sha1 (\S+))?",
@@ -41,7 +41,17 @@
             }
             SYSTEMS.append(pd.DataFrame(data, index=[index]))
             index += 1
 
 # join dfs and drop features without checksums
 SYSTEMS = pd.concat(SYSTEMS)
 SYSTEMS = SYSTEMS[~SYSTEMS["md5"].isnull()].reset_index(drop=True)
+
+# path to retroarch/system (if found)
+RETROARCH_PATH = find_retroarch()
+
+
+# 'cli' if user passes arguments else 'start gui'
+# Needs to be present before the @Gooey decorator (https://github.com/chriskiehl/Gooey/issues/449)
+if len(sys.argv) >= 2:
+    if not "--ignore-gooey" in sys.argv:
+        sys.argv.append("--ignore-gooey")
```

### Comparing `libretro_finder-0.1.3/libretro_finder/main.py` & `libretro_finder-0.2.1/libretro_finder/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-import argparse
 import shutil
 import pathlib
 import numpy as np
-import tqdm
+from gooey import Gooey, GooeyParser
 
 from config import SYSTEMS as system_df
+from config import RETROARCH_PATH
+from typing import List, Optional
 from libretro_finder.utils import match_arrays, recursive_hash
 
 
-def organize(
-    search_dir: pathlib.Path, output_dir: pathlib.Path, glob: str = "*"
-) -> None:
+def organize(search_dir: pathlib.Path, output_dir: pathlib.Path) -> None:
     """
     Non-destructive function that finds, copies and refactors files to the format expected by
     libretro (and its cores). This is useful if you source your BIOS files from many different
     places and have them saved them under different names (often with duplicates).
 
-    :param search_dir:
-    :param output_dir:
-    :param glob:
-    :param overwrite:
+    :param search_dir: starting location of recursive search
+    :param output_dir: path to output directory (will be created if it doesn't exist)
     :return:
     """
 
     # Indexing files to be checked for matching MD5 checksums
     output_dir.mkdir(parents=True, exist_ok=True)
-    file_paths, file_hashes = recursive_hash(directory=search_dir, glob=glob)
+    file_paths, file_hashes = recursive_hash(directory=search_dir)
 
     # Element-wise matching of files against libretro's files
     matching_values, file_indices, system_indices = match_arrays(
         array_a=file_hashes, array_b=np.array(system_df["md5"].values)
     )
 
     if not np.size(matching_values) > 0:
@@ -45,59 +42,69 @@
     # np.unique and indexing doesn't merit a dedicated function but it should still be tested
     assert np.array_equal(np.array(system_subset["md5"].values), hashes)
     assert system_subset["name"].size == system_subset["name"].unique().size
 
     # printing matches per system
     matches = system_subset.groupby("system").count()
     print(
-        f"{matches['name'].sum()} matching BIOS files were found for {matches.shape[0]}"
+        f"{matches['name'].sum()} matching BIOS files were found for {matches.shape[0]} "
         "unique systems:"
     )
     for name, row in matches.iterrows():
         print(f"\t{name} ({row['name']})")
 
     # copying matching files to output_dir using structure specified by libretro
     dsts = system_subset["name"].values
 
     # checking whether our input and output paths are of equal length
     assert len(srcs) == len(dsts)
 
-    for i in tqdm.tqdm(range(srcs.size), total=srcs.size):
+    for i in range(srcs.size):
         dst = output_dir / dsts[i]
         parent = dst.parent
         if dst.exists() or srcs[i] == dst:
             continue
         if parent != output_dir:
             parent.mkdir(parents=True, exist_ok=True)
 
         shutil.copy(src=srcs[i], dst=dst)
 
 
-def main() -> None:
-    """Simple argparse wrapper for packaging."""
-    parser = argparse.ArgumentParser(
-        description="CLI that finds, copies and refactors BIOS files "
-        "to the format expected by libretro (i.e. name and directory structure).",
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+@Gooey(program_name="LibretroFinder", default_size=(610, 530), required_cols=1)
+def main(argv: Optional[List[str]] = None) -> None:
+    """
+    A simple command line utility that finds and prepares your BIOS files for all documented
+    RetroArch cores. If called without any arguments, a simple graphical user interface with
+    the same functionality will be started (courtesy of Gooey).
+    """
+
+    parser = GooeyParser(
+        description="Locate and prepare your BIOS files for libretro.",
     )
-    parser.add_argument("search_dir", help="Directory to look for BIOS files", type=str)
     parser.add_argument(
-        "output_dir", help="Directory to refactor found BIOS files to", type=str
+        "Search directory",
+        help="Where to look for BIOS files",
+        type=pathlib.Path,
+        widget="DirChooser",
     )
     parser.add_argument(
-        "-g",
-        "--glob",
-        help="Glob pattern to use for file matching",
-        type=str,
-        default="*",
+        "Output directory",
+        help="Where to output refactored BIOS files (defaults to ./retroarch/system)",
+        type=pathlib.Path,
+        widget="DirChooser",
+        default=str(RETROARCH_PATH) if RETROARCH_PATH else None,
     )
-    args = vars(parser.parse_args())
+    args = vars(parser.parse_args(argv))
+
+    search_directory = args["Search directory"]
+    output_directory = args["Output directory"]
 
-    search_directory = pathlib.Path(args["search_dir"])
-    output_directory = pathlib.Path(args["output_dir"])
-    search_glob = args["glob"]
+    if not search_directory.exists():
+        raise FileNotFoundError("Search directory does not exist..")
+    elif not search_directory.is_dir():
+        raise NotADirectoryError("Search directory needs to be a directory..")
 
-    organize(search_dir=search_directory, output_dir=output_directory, glob=search_glob)
+    organize(search_dir=search_directory, output_dir=output_directory)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `libretro_finder-0.1.3/LICENSE` & `libretro_finder-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libretro_finder-0.1.3/pyproject.toml` & `libretro_finder-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 [tool.poetry]
 name = "libretro-finder"
-version = "0.1.3"
+version = "0.2.1"
 description = "Command line utility that looks for specific BIOS files for libretro cores and, if found, refactors them to the expected format (i.e. name and directory structure)."
-authors = ["Jasper <j.siebring92@gmail.com>"]
+authors = ["Jasper Siebring <j.siebring92@gmail.com>"]
 license = "GNU General Public License v3.0"
+homepage = "https://github.com/jaspersiebring/libretro_finder"
 readme = "README.md"
 packages = [
     {include = "libretro_finder"},
     {include = "config"},
 ]
 
 [tool.poetry.scripts]
 libretro_finder = "libretro_finder.main:main"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.8,<3.13"
 numpy = "^1.15.0"
 pandas = ">=1.1.5"
 tqdm = "^4.65.0"
+gooey = "^1.0.8.1"
+vdf = "^3.4"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pylint = "^2.17.4"
 black = "^23.7.0"
 mypy = "^1.4.1"
+pyinstaller = "^5.13.0"
+pytest-mock = "^3.11.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pylint.'MESSAGES CONTROL']
 disable = "C0114"
```

