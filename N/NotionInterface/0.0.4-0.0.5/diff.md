# Comparing `tmp/NotionInterface-0.0.4.tar.gz` & `tmp/NotionInterface-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NotionInterface-0.0.4.tar", last modified: Wed Jul 26 16:56:39 2023, max compression
+gzip compressed data, was "NotionInterface-0.0.5.tar", last modified: Mon Jul 31 19:40:52 2023, max compression
```

## Comparing `NotionInterface-0.0.4.tar` & `NotionInterface-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-07-26 16:56:39.037881 NotionInterface-0.0.4/
-drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-07-26 16:56:39.036173 NotionInterface-0.0.4/NotionInterface/
--rw-r--r--   0 lukapedra   (501) staff       (20)      183 2023-07-26 16:55:50.000000 NotionInterface-0.0.4/NotionInterface/__init__.py
--rw-r--r--   0 lukapedra   (501) staff       (20)      213 2023-07-26 16:55:50.000000 NotionInterface-0.0.4/NotionInterface/constants.py
--rw-r--r--   0 lukapedra   (501) staff       (20)     6724 2023-07-26 16:55:50.000000 NotionInterface-0.0.4/NotionInterface/notion_database.py
--rw-r--r--   0 lukapedra   (501) staff       (20)     4871 2023-07-26 16:55:50.000000 NotionInterface-0.0.4/NotionInterface/notion_database_types.py
--rw-r--r--   0 lukapedra   (501) staff       (20)      209 2023-07-26 16:55:50.000000 NotionInterface-0.0.4/NotionInterface/notion_header.py
--rw-r--r--   0 lukapedra   (501) staff       (20)      673 2023-07-26 16:55:50.000000 NotionInterface-0.0.4/NotionInterface/notion_page.py
-drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-07-26 16:56:39.037417 NotionInterface-0.0.4/NotionInterface.egg-info/
--rw-r--r--   0 lukapedra   (501) staff       (20)      573 2023-07-26 16:56:38.000000 NotionInterface-0.0.4/NotionInterface.egg-info/PKG-INFO
--rw-r--r--   0 lukapedra   (501) staff       (20)      409 2023-07-26 16:56:39.000000 NotionInterface-0.0.4/NotionInterface.egg-info/SOURCES.txt
--rw-r--r--   0 lukapedra   (501) staff       (20)        1 2023-07-26 16:56:38.000000 NotionInterface-0.0.4/NotionInterface.egg-info/dependency_links.txt
--rw-r--r--   0 lukapedra   (501) staff       (20)      105 2023-07-26 16:56:38.000000 NotionInterface-0.0.4/NotionInterface.egg-info/requires.txt
--rw-r--r--   0 lukapedra   (501) staff       (20)       16 2023-07-26 16:56:38.000000 NotionInterface-0.0.4/NotionInterface.egg-info/top_level.txt
--rw-r--r--   0 lukapedra   (501) staff       (20)      573 2023-07-26 16:56:39.037701 NotionInterface-0.0.4/PKG-INFO
--rw-r--r--   0 lukapedra   (501) staff       (20)       93 2023-06-20 12:23:58.000000 NotionInterface-0.0.4/README.md
--rw-r--r--   0 lukapedra   (501) staff       (20)       38 2023-07-26 16:56:39.037985 NotionInterface-0.0.4/setup.cfg
--rw-r--r--   0 lukapedra   (501) staff       (20)      858 2023-07-26 16:56:26.000000 NotionInterface-0.0.4/setup.py
+drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-07-31 19:40:52.848262 NotionInterface-0.0.5/
+drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-07-31 19:40:52.846736 NotionInterface-0.0.5/NotionInterface/
+-rw-r--r--   0 lukapedra   (501) staff       (20)      183 2023-07-26 16:55:50.000000 NotionInterface-0.0.5/NotionInterface/__init__.py
+-rw-r--r--   0 lukapedra   (501) staff       (20)      213 2023-07-26 16:55:50.000000 NotionInterface-0.0.5/NotionInterface/constants.py
+-rw-r--r--   0 lukapedra   (501) staff       (20)     6845 2023-07-28 23:03:12.000000 NotionInterface-0.0.5/NotionInterface/notion_database.py
+-rw-r--r--   0 lukapedra   (501) staff       (20)     4871 2023-07-26 16:55:50.000000 NotionInterface-0.0.5/NotionInterface/notion_database_types.py
+-rw-r--r--   0 lukapedra   (501) staff       (20)      209 2023-07-26 16:55:50.000000 NotionInterface-0.0.5/NotionInterface/notion_header.py
+-rw-r--r--   0 lukapedra   (501) staff       (20)      673 2023-07-26 16:55:50.000000 NotionInterface-0.0.5/NotionInterface/notion_page.py
+drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-07-31 19:40:52.847715 NotionInterface-0.0.5/NotionInterface.egg-info/
+-rw-r--r--   0 lukapedra   (501) staff       (20)      509 2023-07-31 19:40:52.000000 NotionInterface-0.0.5/NotionInterface.egg-info/PKG-INFO
+-rw-r--r--   0 lukapedra   (501) staff       (20)      409 2023-07-31 19:40:52.000000 NotionInterface-0.0.5/NotionInterface.egg-info/SOURCES.txt
+-rw-r--r--   0 lukapedra   (501) staff       (20)        1 2023-07-31 19:40:52.000000 NotionInterface-0.0.5/NotionInterface.egg-info/dependency_links.txt
+-rw-r--r--   0 lukapedra   (501) staff       (20)      105 2023-07-31 19:40:52.000000 NotionInterface-0.0.5/NotionInterface.egg-info/requires.txt
+-rw-r--r--   0 lukapedra   (501) staff       (20)       16 2023-07-31 19:40:52.000000 NotionInterface-0.0.5/NotionInterface.egg-info/top_level.txt
+-rw-r--r--   0 lukapedra   (501) staff       (20)      509 2023-07-31 19:40:52.848108 NotionInterface-0.0.5/PKG-INFO
+-rw-r--r--   0 lukapedra   (501) staff       (20)       93 2023-06-20 12:23:58.000000 NotionInterface-0.0.5/README.md
+-rw-r--r--   0 lukapedra   (501) staff       (20)       38 2023-07-31 19:40:52.848306 NotionInterface-0.0.5/setup.cfg
+-rw-r--r--   0 lukapedra   (501) staff       (20)      858 2023-07-31 19:40:30.000000 NotionInterface-0.0.5/setup.py
```

### Comparing `NotionInterface-0.0.4/NotionInterface/notion_database.py` & `NotionInterface-0.0.5/NotionInterface/notion_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,18 @@
             properties = {}
             linha['id'] = res['id']
             linha['created_time'] = res['created_time']
             linha['last_edited_time'] = res['last_edited_time']
 
 
             for key in res['properties'].keys():
-                properties[key] = getValue(res['properties'][key])
+                aux = {}
+                aux['value'] = getValue(res['properties'][key])
+                aux['type'] = res['properties'][key]['type']
+                properties[key] = aux
             linha['properties'] = properties
 
             result.append(linha)
 
         # RECURSÃO PARA PRÓXIMO CURSOR
         if res_dict['next_cursor'] != None:
             result_rec = self.getAllRecords(next_cursor=res_dict['next_cursor'])
```

### Comparing `NotionInterface-0.0.4/NotionInterface/notion_database_types.py` & `NotionInterface-0.0.5/NotionInterface/notion_database_types.py`

 * *Files identical despite different names*

### Comparing `NotionInterface-0.0.4/NotionInterface/notion_page.py` & `NotionInterface-0.0.5/NotionInterface/notion_page.py`

 * *Files identical despite different names*

### Comparing `NotionInterface-0.0.4/setup.py` & `NotionInterface-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'A simple Notion db interface for Python'
 requirements = []
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 # Setting up
 setup(
```

