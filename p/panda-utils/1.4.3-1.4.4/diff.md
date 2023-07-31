# Comparing `tmp/panda_utils-1.4.3.tar.gz` & `tmp/panda_utils-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda_utils-1.4.3.tar", last modified: Mon Jul 31 00:35:46 2023, max compression
+gzip compressed data, was "panda_utils-1.4.4.tar", last modified: Mon Jul 31 21:46:45 2023, max compression
```

## Comparing `panda_utils-1.4.3.tar` & `panda_utils-1.4.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-31 00:35:46.591543 panda_utils-1.4.3/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1085 2023-07-07 08:54:13.000000 panda_utils-1.4.3/LICENSE
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-07-31 00:35:46.591543 panda_utils-1.4.3/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1476 2023-07-11 16:19:27.000000 panda_utils-1.4.3/README.md
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.4.3/config_example.ini
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-31 00:35:46.588210 panda_utils-1.4.3/panda_utils/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.4.3/panda_utils/__init__.py
--rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.4.3/panda_utils/__main__.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-31 00:35:46.588210 panda_utils-1.4.3/panda_utils/assetpipeline/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.4.3/panda_utils/assetpipeline/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5006 2023-07-31 00:27:55.000000 panda_utils-1.4.3/panda_utils/assetpipeline/__main__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      247 2023-07-28 09:44:44.000000 panda_utils-1.4.3/panda_utils/assetpipeline/imports.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      747 2023-07-30 10:56:09.000000 panda_utils-1.4.3/panda_utils/assetpipeline/misc.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    14795 2023-07-30 23:14:46.000000 panda_utils-1.4.3/panda_utils/assetpipeline/models.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      785 2023-06-13 10:37:09.000000 panda_utils-1.4.3/panda_utils/assetpipeline/textures.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-31 00:35:46.591543 panda_utils-1.4.3/panda_utils/blender/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.4.3/panda_utils/blender/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      615 2023-07-28 09:44:44.000000 panda_utils-1.4.3/panda_utils/blender/export_glb.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1797 2023-07-28 09:44:44.000000 panda_utils-1.4.3/panda_utils/blender/export_with_yabee.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      527 2023-07-28 09:44:44.000000 panda_utils-1.4.3/panda_utils/blender/import_model.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      454 2023-07-11 08:56:38.000000 panda_utils-1.4.3/panda_utils/blender/patch_paths.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-31 00:35:46.591543 panda_utils-1.4.3/panda_utils/eggtree/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.4.3/panda_utils/eggtree/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5632 2023-07-28 09:44:44.000000 panda_utils-1.4.3/panda_utils/eggtree/eggparse.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      762 2023-07-25 21:42:36.000000 panda_utils-1.4.3/panda_utils/eggtree/operations.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-31 00:35:46.591543 panda_utils-1.4.3/panda_utils/tools/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.4.3/panda_utils/tools/__init__.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.4.3/panda_utils/tools/animconvert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5397 2023-06-12 17:52:50.000000 panda_utils-1.4.3/panda_utils/tools/convert.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3686 2023-06-13 10:30:48.000000 panda_utils-1.4.3/panda_utils/tools/downscale.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3201 2023-06-13 12:07:52.000000 panda_utils-1.4.3/panda_utils/tools/palettize.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.4.3/panda_utils/tools/toontown.py
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3332 2023-07-08 05:28:59.000000 panda_utils-1.4.3/panda_utils/util.py
-drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-31 00:35:46.588210 panda_utils-1.4.3/panda_utils.egg-info/
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-07-31 00:35:46.000000 panda_utils-1.4.3/panda_utils.egg-info/PKG-INFO
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      991 2023-07-31 00:35:46.000000 panda_utils-1.4.3/panda_utils.egg-info/SOURCES.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-07-31 00:35:46.000000 panda_utils-1.4.3/panda_utils.egg-info/dependency_links.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-07-31 00:35:46.000000 panda_utils-1.4.3/panda_utils.egg-info/requires.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-07-31 00:35:46.000000 panda_utils-1.4.3/panda_utils.egg-info/top_level.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1023 2023-07-31 00:35:01.000000 panda_utils-1.4.3/pyproject.toml
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.4.3/requirements.txt
--rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-07-31 00:35:46.591543 panda_utils-1.4.3/setup.cfg
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-31 21:46:45.646411 panda_utils-1.4.4/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1085 2023-07-07 08:54:13.000000 panda_utils-1.4.4/LICENSE
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-07-31 21:46:45.646411 panda_utils-1.4.4/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1476 2023-07-11 16:19:27.000000 panda_utils-1.4.4/README.md
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      327 2023-06-11 07:33:25.000000 panda_utils-1.4.4/config_example.ini
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-31 21:46:45.643077 panda_utils-1.4.4/panda_utils/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.4.4/panda_utils/__init__.py
+-rwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)     6345 2023-06-11 07:03:04.000000 panda_utils-1.4.4/panda_utils/__main__.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-31 21:46:45.643077 panda_utils-1.4.4/panda_utils/assetpipeline/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 07:03:50.000000 panda_utils-1.4.4/panda_utils/assetpipeline/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5006 2023-07-31 00:27:55.000000 panda_utils-1.4.4/panda_utils/assetpipeline/__main__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      247 2023-07-28 09:44:44.000000 panda_utils-1.4.4/panda_utils/assetpipeline/imports.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      747 2023-07-30 10:56:09.000000 panda_utils-1.4.4/panda_utils/assetpipeline/misc.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)    15470 2023-07-31 21:33:06.000000 panda_utils-1.4.4/panda_utils/assetpipeline/models.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      785 2023-06-13 10:37:09.000000 panda_utils-1.4.4/panda_utils/assetpipeline/textures.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-31 21:46:45.643077 panda_utils-1.4.4/panda_utils/blender/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-06-11 08:19:46.000000 panda_utils-1.4.4/panda_utils/blender/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      615 2023-07-28 09:44:44.000000 panda_utils-1.4.4/panda_utils/blender/export_glb.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1797 2023-07-28 09:44:44.000000 panda_utils-1.4.4/panda_utils/blender/export_with_yabee.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      527 2023-07-28 09:44:44.000000 panda_utils-1.4.4/panda_utils/blender/import_model.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      454 2023-07-11 08:56:38.000000 panda_utils-1.4.4/panda_utils/blender/patch_paths.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-31 21:46:45.646411 panda_utils-1.4.4/panda_utils/eggtree/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-09-19 11:38:19.000000 panda_utils-1.4.4/panda_utils/eggtree/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5632 2023-07-28 09:44:44.000000 panda_utils-1.4.4/panda_utils/eggtree/eggparse.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      762 2023-07-25 21:42:36.000000 panda_utils-1.4.4/panda_utils/eggtree/operations.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-31 21:46:45.646411 panda_utils-1.4.4/panda_utils/tools/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        0 2022-08-12 11:48:21.000000 panda_utils-1.4.4/panda_utils/tools/__init__.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1449 2023-06-10 09:05:07.000000 panda_utils-1.4.4/panda_utils/tools/animconvert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     5397 2023-06-12 17:52:50.000000 panda_utils-1.4.4/panda_utils/tools/convert.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3686 2023-06-13 10:30:48.000000 panda_utils-1.4.4/panda_utils/tools/downscale.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3201 2023-06-13 12:07:52.000000 panda_utils-1.4.4/panda_utils/tools/palettize.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1373 2023-06-10 09:05:07.000000 panda_utils-1.4.4/panda_utils/tools/toontown.py
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     3332 2023-07-08 05:28:59.000000 panda_utils-1.4.4/panda_utils/util.py
+drwxr-xr-x   0 wizzerinus  (1000) wizzerinus  (1000)        0 2023-07-31 21:46:45.643077 panda_utils-1.4.4/panda_utils.egg-info/
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     2206 2023-07-31 21:46:45.000000 panda_utils-1.4.4/panda_utils.egg-info/PKG-INFO
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      991 2023-07-31 21:46:45.000000 panda_utils-1.4.4/panda_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)        1 2023-07-31 21:46:45.000000 panda_utils-1.4.4/panda_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)      274 2023-07-31 21:46:45.000000 panda_utils-1.4.4/panda_utils.egg-info/requires.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       12 2023-07-31 21:46:45.000000 panda_utils-1.4.4/panda_utils.egg-info/top_level.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)     1023 2023-07-31 21:46:34.000000 panda_utils-1.4.4/pyproject.toml
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       66 2023-06-11 07:37:00.000000 panda_utils-1.4.4/requirements.txt
+-rw-r--r--   0 wizzerinus  (1000) wizzerinus  (1000)       38 2023-07-31 21:46:45.646411 panda_utils-1.4.4/setup.cfg
```

### Comparing `panda_utils-1.4.3/LICENSE` & `panda_utils-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.3/PKG-INFO` & `panda_utils-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda_utils
-Version: 1.4.3
+Version: 1.4.4
 Summary: PandaUtils includes multiple tools for basic Panda3D automation
 Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
 Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
 Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `panda_utils-1.4.3/README.md` & `panda_utils-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.3/panda_utils/__main__.py` & `panda_utils-1.4.4/panda_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.3/panda_utils/assetpipeline/__main__.py` & `panda_utils-1.4.4/panda_utils/assetpipeline/__main__.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.3/panda_utils/assetpipeline/misc.py` & `panda_utils-1.4.4/panda_utils/assetpipeline/misc.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.3/panda_utils/assetpipeline/models.py` & `panda_utils-1.4.4/panda_utils/assetpipeline/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,17 @@
     stdout_pipe = subprocess.DEVNULL if not os.getenv("PANDA_UTILS_BLENDER_LOGGING") else None
     subprocess.run(args, stdout=stdout_pipe, cwd=cwd)
 
 
 def build_asset_mapper(assets, name):
     output = {}
     for counter, item in enumerate(sorted(assets)):
+        if "_palette_" in item:
+            continue
+
         extension = item.split(".")[-1]
         new_file_name = f"{name}-{counter}.{extension}" if counter else f"{name}.{extension}"
         output[item] = new_file_name
     return output
 
 
 def __patch_filename(filename):
@@ -241,15 +244,15 @@
     group_name = group_name or ctx.model_name
     method = method.capitalize()
     flags = flags.replace(",", " ")
     ctx.cache_eggs()
     for file, eggtree in ctx.eggs.items():
         logger.info("%s: Adding collisions to %s/%s: flags=%s method=%s", ctx.name, file, group_name, flags, method)
         groups = [group for group in eggtree.findall("Group") if group.node_name == group_name]
-        if len(groups) == 1:
+        if groups:
             logger.info("Found the named group!")
             new_node = eggparse.EggLeaf("Collide", group_name, f"{method} {flags}")
             group_children = groups[0].children.children
             group_children.insert(0, new_node)
 
             if bitmask is not None:
                 mask_hex = f"{bitmask:#010x}"
@@ -261,30 +264,46 @@
             # https://github.com/panda3d/panda3d/issues/1515
             nodes = groups[0].findall("Line") + groups[0].findall("Patch") + groups[0].findall("PointLight")
             if nodes:
                 logger.warning("Found non-polygon objects while generating collisions, removing...")
                 groups[0].remove_nodes(set(nodes))
 
 
-def action_palettize(ctx, palette_size="1024", flags=""):
+def action_palettize(ctx, palette_size="1024", flags="", exclusions=""):
     ctx.uncache_eggs()
     palette_size = int(palette_size)
     if palette_size & (palette_size - 1):
         raise ValueError("The palette size must be a power of two!")
 
     flag_list = flags.split(",")
 
     logger.info("%s: Creating a TXA file...", ctx.name)
     txa_text = (
         f":palette {palette_size} {palette_size}\n"
         ":imagetype png\n"
         ":powertwo 1\n"
         f":group {ctx.model_name} dir .\n"
-        f"*.png : force-rgba dual linear clamp_u clamp_v margin 5\n"
     )
+    if isinstance(exclusions, str):
+        exclusions = list(filter(None, exclusions.split(",")))
+
+    all_png_files = [file for file in ctx.files if file.endswith(".png")]
+    included_png_files, excluded_png_files = [], []
+    for file in all_png_files:
+        if file in exclusions:
+            excluded_png_files.append(file)
+        else:
+            included_png_files.append(file)
+
+    if not included_png_files:
+        raise RuntimeError("No images were included in the palette!")
+    txa_text += " ".join(included_png_files) + " : force-rgba dual linear clamp_u clamp_v margin 5\n"
+    if excluded_png_files:
+        txa_text += " ".join(excluded_png_files) + " : omit\n"
+
     with open("textures.txa", "w") as txa_file:
         txa_file.write(txa_text)
 
     all_eggs = [file for file in ctx.files if file.endswith(".egg")]
 
     logger.info("%s: Palettizing %s...", ctx.name, ", ".join(all_eggs))
     util.run_panda(
```

### Comparing `panda_utils-1.4.3/panda_utils/assetpipeline/textures.py` & `panda_utils-1.4.4/panda_utils/assetpipeline/textures.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.3/panda_utils/blender/export_glb.py` & `panda_utils-1.4.4/panda_utils/blender/export_glb.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.3/panda_utils/blender/export_with_yabee.py` & `panda_utils-1.4.4/panda_utils/blender/export_with_yabee.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.3/panda_utils/blender/import_model.py` & `panda_utils-1.4.4/panda_utils/blender/import_model.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.3/panda_utils/eggtree/eggparse.py` & `panda_utils-1.4.4/panda_utils/eggtree/eggparse.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.3/panda_utils/eggtree/operations.py` & `panda_utils-1.4.4/panda_utils/eggtree/operations.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.3/panda_utils/tools/animconvert.py` & `panda_utils-1.4.4/panda_utils/tools/animconvert.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.3/panda_utils/tools/convert.py` & `panda_utils-1.4.4/panda_utils/tools/convert.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.3/panda_utils/tools/downscale.py` & `panda_utils-1.4.4/panda_utils/tools/downscale.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.3/panda_utils/tools/palettize.py` & `panda_utils-1.4.4/panda_utils/tools/palettize.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.3/panda_utils/tools/toontown.py` & `panda_utils-1.4.4/panda_utils/tools/toontown.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.3/panda_utils/util.py` & `panda_utils-1.4.4/panda_utils/util.py`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.3/panda_utils.egg-info/PKG-INFO` & `panda_utils-1.4.4/panda_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda-utils
-Version: 1.4.3
+Version: 1.4.4
 Summary: PandaUtils includes multiple tools for basic Panda3D automation
 Author-email: "Toontown: Event Horizon" <development@toontowneventhorizon.com>
 Project-URL: homepage, https://github.com/toontown-event-horizon/panda-utils
 Project-URL: bugtracker, https://github.com/toontown-event-horizon/panda-utils/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `panda_utils-1.4.3/panda_utils.egg-info/SOURCES.txt` & `panda_utils-1.4.4/panda_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panda_utils-1.4.3/pyproject.toml` & `panda_utils-1.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=60", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "panda_utils"
-version = "1.4.3"
+version = "1.4.4"
 authors = [
     {name = "Toontown: Event Horizon", email = "development@toontowneventhorizon.com"}
 ]
 description = "PandaUtils includes multiple tools for basic Panda3D automation"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

