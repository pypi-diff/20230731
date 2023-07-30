# Comparing `tmp/nichord-0.2.1.tar.gz` & `tmp/nichord-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nichord-0.2.1.tar", last modified: Sun Jul 30 21:57:32 2023, max compression
+gzip compressed data, was "nichord-0.2.2.tar", last modified: Sun Jul 30 22:01:01 2023, max compression
```

## Comparing `nichord-0.2.1.tar` & `nichord-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 21:57:32.648187 nichord-0.2.1/
--rw-rw-rw-   0        0        0     1570 2023-07-30 21:57:32.647186 nichord-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     9250 2023-07-30 21:49:33.000000 nichord-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 21:57:32.642185 nichord-0.2.1/nichord/
--rw-rw-rw-   0        0        0      756 2022-11-12 03:49:12.000000 nichord-0.2.1/nichord/__init__.py
--rw-rw-rw-   0        0        0    34573 2023-07-30 17:47:59.000000 nichord-0.2.1/nichord/chord.py
--rw-rw-rw-   0        0        0     4893 2022-11-13 19:54:36.000000 nichord-0.2.1/nichord/combine.py
--rw-rw-rw-   0        0        0      482 2022-05-22 13:31:30.000000 nichord-0.2.1/nichord/convert.py
--rw-rw-rw-   0        0        0     5683 2023-07-30 02:58:52.000000 nichord-0.2.1/nichord/coord_labeler.py
--rw-rw-rw-   0        0        0     5731 2022-11-12 03:52:39.000000 nichord-0.2.1/nichord/glassbrain.py
--rw-rw-rw-   0        0        0     2156 2023-07-24 20:52:49.000000 nichord-0.2.1/nichord/patch_RendererAgg.py
-drwxrwxrwx   0        0        0        0 2023-07-30 21:57:32.646186 nichord-0.2.1/nichord.egg-info/
--rw-rw-rw-   0        0        0     1570 2023-07-30 21:57:32.000000 nichord-0.2.1/nichord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-07-30 21:57:32.000000 nichord-0.2.1/nichord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 21:57:32.000000 nichord-0.2.1/nichord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-30 21:57:32.000000 nichord-0.2.1/nichord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-30 21:57:32.000000 nichord-0.2.1/nichord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 21:57:32.648187 nichord-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     2199 2023-07-30 21:56:40.000000 nichord-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 22:01:01.703082 nichord-0.2.2/
+-rw-rw-rw-   0        0        0      850 2023-07-30 22:01:01.703082 nichord-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9250 2023-07-30 21:49:33.000000 nichord-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-30 22:01:01.697081 nichord-0.2.2/nichord/
+-rw-rw-rw-   0        0        0      756 2022-11-12 03:49:12.000000 nichord-0.2.2/nichord/__init__.py
+-rw-rw-rw-   0        0        0    34573 2023-07-30 17:47:59.000000 nichord-0.2.2/nichord/chord.py
+-rw-rw-rw-   0        0        0     4893 2022-11-13 19:54:36.000000 nichord-0.2.2/nichord/combine.py
+-rw-rw-rw-   0        0        0      482 2022-05-22 13:31:30.000000 nichord-0.2.2/nichord/convert.py
+-rw-rw-rw-   0        0        0     5683 2023-07-30 02:58:52.000000 nichord-0.2.2/nichord/coord_labeler.py
+-rw-rw-rw-   0        0        0     5731 2022-11-12 03:52:39.000000 nichord-0.2.2/nichord/glassbrain.py
+-rw-rw-rw-   0        0        0     2156 2023-07-24 20:52:49.000000 nichord-0.2.2/nichord/patch_RendererAgg.py
+drwxrwxrwx   0        0        0        0 2023-07-30 22:01:01.702082 nichord-0.2.2/nichord.egg-info/
+-rw-rw-rw-   0        0        0      850 2023-07-30 22:01:01.000000 nichord-0.2.2/nichord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-07-30 22:01:01.000000 nichord-0.2.2/nichord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 22:01:01.000000 nichord-0.2.2/nichord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-30 22:01:01.000000 nichord-0.2.2/nichord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-30 22:01:01.000000 nichord-0.2.2/nichord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 22:01:01.704083 nichord-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1530 2023-07-30 22:00:49.000000 nichord-0.2.2/setup.py
```

### Comparing `nichord-0.2.1/README.md` & `nichord-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nichord-0.2.1/nichord/__init__.py` & `nichord-0.2.2/nichord/__init__.py`

 * *Files identical despite different names*

### Comparing `nichord-0.2.1/nichord/chord.py` & `nichord-0.2.2/nichord/chord.py`

 * *Files identical despite different names*

### Comparing `nichord-0.2.1/nichord/combine.py` & `nichord-0.2.2/nichord/combine.py`

 * *Files identical despite different names*

### Comparing `nichord-0.2.1/nichord/coord_labeler.py` & `nichord-0.2.2/nichord/coord_labeler.py`

 * *Files identical despite different names*

### Comparing `nichord-0.2.1/nichord/glassbrain.py` & `nichord-0.2.2/nichord/glassbrain.py`

 * *Files identical despite different names*

### Comparing `nichord-0.2.1/nichord/patch_RendererAgg.py` & `nichord-0.2.2/nichord/patch_RendererAgg.py`

 * *Files identical despite different names*

