# Comparing `tmp/ydl_podcast-1.2.1.tar.gz` & `tmp/ydl_podcast-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydl_podcast-1.2.1.tar", max compression
+gzip compressed data, was "ydl_podcast-1.2.2.tar", max compression
```

## Comparing `ydl_podcast-1.2.1.tar` & `ydl_podcast-1.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1102 2023-07-30 02:46:39.227326 ydl_podcast-1.2.1/LICENSE
--rw-r--r--   0        0        0     3100 2023-07-30 02:46:39.227326 ydl_podcast-1.2.1/README.md
--rw-r--r--   0        0        0      915 2023-07-30 22:04:09.395650 ydl_podcast-1.2.1/pyproject.toml
--rw-r--r--   0        0        0    15098 2023-07-30 22:04:09.395650 ydl_podcast-1.2.1/ydl_podcast/__init__.py
--rwxr-xr-x   0        0        0     1872 2023-07-30 02:46:39.227326 ydl_podcast-1.2.1/ydl_podcast/__main__.py
--rw-r--r--   0        0        0     1482 2023-07-30 02:46:39.227326 ydl_podcast-1.2.1/ydl_podcast/template.py
--rw-r--r--   0        0        0     4223 1970-01-01 00:00:00.000000 ydl_podcast-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-07-30 02:46:39.227326 ydl_podcast-1.2.2/LICENSE
+-rw-r--r--   0        0        0     3100 2023-07-30 02:46:39.227326 ydl_podcast-1.2.2/README.md
+-rw-r--r--   0        0        0      915 2023-07-31 02:54:25.346632 ydl_podcast-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0    15246 2023-07-31 02:54:25.346632 ydl_podcast-1.2.2/ydl_podcast/__init__.py
+-rwxr-xr-x   0        0        0     1872 2023-07-30 02:46:39.227326 ydl_podcast-1.2.2/ydl_podcast/__main__.py
+-rw-r--r--   0        0        0     1482 2023-07-30 02:46:39.227326 ydl_podcast-1.2.2/ydl_podcast/template.py
+-rw-r--r--   0        0        0     4223 1970-01-01 00:00:00.000000 ydl_podcast-1.2.2/PKG-INFO
```

### Comparing `ydl_podcast-1.2.1/LICENSE` & `ydl_podcast-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.2.1/README.md` & `ydl_podcast-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.2.1/pyproject.toml` & `ydl_podcast-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ydl-podcast"
-version = "1.2.1"
+version = "1.2.2"
 description = "A simple tool to generate Podcast-like RSS feeds from youtube (or other youtube-dl supported services) channels, using youtube-dl"
 license = "MIT"
 authors = ["nbr23 <max@23.tf>"]
 homepage = "https://github.com/nbr23/ydl-podcast"
 repository = "https://github.com/nbr23/ydl-podcast"
 keywords = ["podcast", "youtube-dl"]
 readme = "README.md"
```

### Comparing `ydl_podcast-1.2.1/ydl_podcast/__init__.py` & `ydl_podcast-1.2.2/ydl_podcast/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -396,19 +396,22 @@
                 "url": "/".join(
                     [sub["url_root"], quote(sub["name"]), quote(md["filename"])]
                 ),
                 "media_type": ("audio/%s" % md["extension"])
                 if sub["audio_only"]
                 else "video/%s" % md["extension"],
                 "pubDate": md["pub_date"],
-                "thumbnail": "/".join(
-                    [sub["url_root"], quote(sub["name"]), quote(md["thumbnail"])]
-                )
-                if md.get("thumbnail") is not None
-                else None,
+                "thumbnail": "/".join([
+                    sub["url_root"],
+                    quote(sub["name"]),
+                    quote(convert_thumbnail_to_jpg(
+                        os.path.join(sub["url_root"], sub["name"]),
+                        md["thumbnail"]
+                    ))
+                ]) if md.get("thumbnail") is not None else None,
                 "description": md["description"],
                 "duration": md["duration"],
             }
             for md in mds
         ],
     }
```

### Comparing `ydl_podcast-1.2.1/ydl_podcast/__main__.py` & `ydl_podcast-1.2.2/ydl_podcast/__main__.py`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.2.1/ydl_podcast/template.py` & `ydl_podcast-1.2.2/ydl_podcast/template.py`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.2.1/PKG-INFO` & `ydl_podcast-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydl-podcast
-Version: 1.2.1
+Version: 1.2.2
 Summary: A simple tool to generate Podcast-like RSS feeds from youtube (or other youtube-dl supported services) channels, using youtube-dl
 Home-page: https://github.com/nbr23/ydl-podcast
 License: MIT
 Keywords: podcast,youtube-dl
 Author: nbr23
 Author-email: max@23.tf
 Requires-Python: >=3.7,<4.0
```

