# Comparing `tmp/ydl_podcast-1.2.0.tar.gz` & `tmp/ydl_podcast-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydl_podcast-1.2.0.tar", max compression
+gzip compressed data, was "ydl_podcast-1.2.1.tar", max compression
```

## Comparing `ydl_podcast-1.2.0.tar` & `ydl_podcast-1.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1102 2023-07-30 02:46:39.227326 ydl_podcast-1.2.0/LICENSE
--rw-r--r--   0        0        0     3100 2023-07-30 02:46:39.227326 ydl_podcast-1.2.0/README.md
--rw-r--r--   0        0        0      915 2023-07-30 18:09:37.140643 ydl_podcast-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    15033 2023-07-30 18:09:37.140643 ydl_podcast-1.2.0/ydl_podcast/__init__.py
--rwxr-xr-x   0        0        0     1872 2023-07-30 02:46:39.227326 ydl_podcast-1.2.0/ydl_podcast/__main__.py
--rw-r--r--   0        0        0     1482 2023-07-30 02:46:39.227326 ydl_podcast-1.2.0/ydl_podcast/template.py
--rw-r--r--   0        0        0     4223 1970-01-01 00:00:00.000000 ydl_podcast-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-07-30 02:46:39.227326 ydl_podcast-1.2.1/LICENSE
+-rw-r--r--   0        0        0     3100 2023-07-30 02:46:39.227326 ydl_podcast-1.2.1/README.md
+-rw-r--r--   0        0        0      915 2023-07-30 22:04:09.395650 ydl_podcast-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    15098 2023-07-30 22:04:09.395650 ydl_podcast-1.2.1/ydl_podcast/__init__.py
+-rwxr-xr-x   0        0        0     1872 2023-07-30 02:46:39.227326 ydl_podcast-1.2.1/ydl_podcast/__main__.py
+-rw-r--r--   0        0        0     1482 2023-07-30 02:46:39.227326 ydl_podcast-1.2.1/ydl_podcast/template.py
+-rw-r--r--   0        0        0     4223 1970-01-01 00:00:00.000000 ydl_podcast-1.2.1/PKG-INFO
```

### Comparing `ydl_podcast-1.2.0/LICENSE` & `ydl_podcast-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.2.0/README.md` & `ydl_podcast-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.2.0/pyproject.toml` & `ydl_podcast-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ydl-podcast"
-version = "1.2.0"
+version = "1.2.1"
 description = "A simple tool to generate Podcast-like RSS feeds from youtube (or other youtube-dl supported services) channels, using youtube-dl"
 license = "MIT"
 authors = ["nbr23 <max@23.tf>"]
 homepage = "https://github.com/nbr23/ydl-podcast"
 repository = "https://github.com/nbr23/ydl-podcast"
 keywords = ["podcast", "youtube-dl"]
 readme = "README.md"
```

### Comparing `ydl_podcast-1.2.0/ydl_podcast/__init__.py` & `ydl_podcast-1.2.1/ydl_podcast/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 
 
 def convert_thumbnail_to_jpg(path, thumbnail_filename):
     ext = thumbnail_filename.split(".")[-1]
     if ext == "jpg" or ext == "jpeg":
         return thumbnail_filename
     try:
+        print("Converting thumbnail to jpg", thumbnail_filename)
         im = Image.open(os.path.join(path, thumbnail_filename))
         rgb_im = im.convert("RGB")
         new_thumbnail_filename = thumbnail_filename.replace("."+ext, ".jpg")
         rgb_im.save(os.path.join(path, new_thumbnail_filename))
         os.remove(os.path.join(path, thumbnail_filename))
         return new_thumbnail_filename
     except Exception as e:
```

### Comparing `ydl_podcast-1.2.0/ydl_podcast/__main__.py` & `ydl_podcast-1.2.1/ydl_podcast/__main__.py`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.2.0/ydl_podcast/template.py` & `ydl_podcast-1.2.1/ydl_podcast/template.py`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.2.0/PKG-INFO` & `ydl_podcast-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydl-podcast
-Version: 1.2.0
+Version: 1.2.1
 Summary: A simple tool to generate Podcast-like RSS feeds from youtube (or other youtube-dl supported services) channels, using youtube-dl
 Home-page: https://github.com/nbr23/ydl-podcast
 License: MIT
 Keywords: podcast,youtube-dl
 Author: nbr23
 Author-email: max@23.tf
 Requires-Python: >=3.7,<4.0
```

