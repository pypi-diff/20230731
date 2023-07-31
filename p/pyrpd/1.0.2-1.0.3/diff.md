# Comparing `tmp/pyrpd-1.0.2.tar.gz` & `tmp/pyrpd-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyrpd-1.0.2.tar", last modified: Thu Mar  9 03:23:00 2023, max compression
+gzip compressed data, was "pyrpd-1.0.3.tar", last modified: Mon Jul 31 08:42:28 2023, max compression
```

## Comparing `pyrpd-1.0.2.tar` & `pyrpd-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 03:23:00.434944 pyrpd-1.0.2/
--rw-rw-rw-   0        0        0     1088 2023-03-07 02:05:06.000000 pyrpd-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      160 2023-03-07 02:51:36.000000 pyrpd-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1536 2023-03-09 03:23:00.434944 pyrpd-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      923 2023-03-09 02:37:25.000000 pyrpd-1.0.2/README.md
--rw-rw-rw-   0        0        0      233 2023-03-07 02:50:38.000000 pyrpd-1.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-03-09 03:23:00.409166 pyrpd-1.0.2/pyrpd/
--rw-rw-rw-   0        0        0      172 2023-03-07 06:43:00.000000 pyrpd-1.0.2/pyrpd/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-09 03:23:00.429957 pyrpd-1.0.2/pyrpd/tests/
--rw-rw-rw-   0        0        0       82 2023-03-07 07:00:52.000000 pyrpd-1.0.2/pyrpd/tests/__init__.py
--rw-rw-rw-   0        0        0     1186 2023-03-09 02:37:25.000000 pyrpd-1.0.2/pyrpd/tests/wechat.py
-drwxrwxrwx   0        0        0        0 2023-03-09 03:23:00.423971 pyrpd-1.0.2/pyrpd.egg-info/
--rw-rw-rw-   0        0        0     1536 2023-03-09 03:23:00.000000 pyrpd-1.0.2/pyrpd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-03-09 03:23:00.000000 pyrpd-1.0.2/pyrpd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 03:23:00.000000 pyrpd-1.0.2/pyrpd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-03-09 03:23:00.000000 pyrpd-1.0.2/pyrpd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      184 2023-03-09 03:23:00.437765 pyrpd-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1562 2023-03-09 03:13:18.000000 pyrpd-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-09 03:23:00.401187 pyrpd-1.0.2/source/
--rw-rw-rw-   0        0        0   293912 2023-03-09 03:23:00.000000 pyrpd-1.0.2/source/_pyrpd.cpp
+drwxrwxrwx   0        0        0        0 2023-07-31 08:42:28.461245 pyrpd-1.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-03-07 02:05:06.000000 pyrpd-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      160 2023-03-07 02:51:36.000000 pyrpd-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1810 2023-07-31 08:42:28.461245 pyrpd-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      923 2023-03-09 02:37:25.000000 pyrpd-1.0.3/README.md
+-rw-rw-rw-   0        0        0      233 2023-03-07 02:50:38.000000 pyrpd-1.0.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-31 08:42:28.461245 pyrpd-1.0.3/pyrpd/
+-rw-rw-rw-   0        0        0      172 2023-03-07 06:43:00.000000 pyrpd-1.0.3/pyrpd/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 08:42:28.461245 pyrpd-1.0.3/pyrpd/tests/
+-rw-rw-rw-   0        0        0       82 2023-03-07 07:00:52.000000 pyrpd-1.0.3/pyrpd/tests/__init__.py
+-rw-rw-rw-   0        0        0     1204 2023-07-28 10:00:25.000000 pyrpd-1.0.3/pyrpd/tests/wechat.py
+drwxrwxrwx   0        0        0        0 2023-07-31 08:42:28.461245 pyrpd-1.0.3/pyrpd.egg-info/
+-rw-rw-rw-   0        0        0     1810 2023-07-31 08:42:28.000000 pyrpd-1.0.3/pyrpd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-07-31 08:42:28.000000 pyrpd-1.0.3/pyrpd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 08:42:28.000000 pyrpd-1.0.3/pyrpd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-31 08:42:28.000000 pyrpd-1.0.3/pyrpd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      184 2023-07-31 08:42:28.461245 pyrpd-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1562 2023-07-28 10:13:34.000000 pyrpd-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 08:42:28.461245 pyrpd-1.0.3/source/
+-rw-rw-rw-   0        0        0   511419 2023-07-28 10:06:50.000000 pyrpd-1.0.3/source/_pyrpd.cpp
```

### Comparing `pyrpd-1.0.2/LICENSE` & `pyrpd-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrpd-1.0.2/README.md` & `pyrpd-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyrpd-1.0.2/pyrpd/tests/wechat.py` & `pyrpd-1.0.3/pyrpd/tests/wechat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pyrpd
 
 class WeChat(pyrpd.PyRProcess):
     def __init__(self,pid,*args,**kwargs):
-        super().__init__()
+        super().__init__(pid,*args,**kwargs)
         
     @classmethod
     def new_wechat(cls):
         return cls(pyrpd.new_wechat())
     
     def load(self,*args,**kwargs):
         return super().load(*args,**kwargs)
```

### Comparing `pyrpd-1.0.2/setup.py` & `pyrpd-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
               include_dirs=["../","."],
               define_macros=define_macros,
               language="c++"),
     ]
 
 setup(
     name="pyrpd",
-    version="1.0.2",
+    version="1.0.3",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Jack Li",
     author_email="ljc545w@qq.com",
     url='https://github.com/ljc545w/pyrpd',
     install_requires=[],
     license="MIT License",
```

