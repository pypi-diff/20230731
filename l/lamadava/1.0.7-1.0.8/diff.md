# Comparing `tmp/lamadava-1.0.7.tar.gz` & `tmp/lamadava-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamadava-1.0.7.tar", last modified: Fri Jul 28 19:34:40 2023, max compression
+gzip compressed data, was "lamadava-1.0.8.tar", last modified: Mon Jul 31 17:12:35 2023, max compression
```

## Comparing `lamadava-1.0.7.tar` & `lamadava-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-07-28 19:34:40.269343 lamadava-1.0.7/
--rw-r--r--   0 adw0rd     (501) staff       (20)     1072 2023-05-11 17:49:04.000000 lamadava-1.0.7/LICENSE
--rw-r--r--   0 adw0rd     (501) staff       (20)     1720 2023-07-28 19:34:40.269219 lamadava-1.0.7/PKG-INFO
--rw-r--r--   0 adw0rd     (501) staff       (20)      670 2023-05-22 11:50:12.000000 lamadava-1.0.7/README.md
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-07-28 19:34:40.268533 lamadava-1.0.7/lamadava/
--rw-r--r--   0 adw0rd     (501) staff       (20)      451 2023-06-05 21:44:38.000000 lamadava-1.0.7/lamadava/__init__.py
--rw-r--r--   0 adw0rd     (501) staff       (20)       96 2023-07-28 19:33:45.000000 lamadava-1.0.7/lamadava/__version__.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    30131 2023-07-28 19:28:54.000000 lamadava-1.0.7/lamadava/api.py
--rw-r--r--   0 adw0rd     (501) staff       (20)    31422 2023-07-28 19:28:54.000000 lamadava-1.0.7/lamadava/asyncapi.py
--rw-r--r--   0 adw0rd     (501) staff       (20)     5631 2023-07-28 19:28:52.000000 lamadava-1.0.7/lamadava/base.py
-drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-07-28 19:34:40.269052 lamadava-1.0.7/lamadava.egg-info/
--rw-r--r--   0 adw0rd     (501) staff       (20)     1720 2023-07-28 19:34:40.000000 lamadava-1.0.7/lamadava.egg-info/PKG-INFO
--rw-r--r--   0 adw0rd     (501) staff       (20)      284 2023-07-28 19:34:40.000000 lamadava-1.0.7/lamadava.egg-info/SOURCES.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)        1 2023-07-28 19:34:40.000000 lamadava-1.0.7/lamadava.egg-info/dependency_links.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)       14 2023-07-28 19:34:40.000000 lamadava-1.0.7/lamadava.egg-info/requires.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)        9 2023-07-28 19:34:40.000000 lamadava-1.0.7/lamadava.egg-info/top_level.txt
--rw-r--r--   0 adw0rd     (501) staff       (20)       38 2023-07-28 19:34:40.269379 lamadava-1.0.7/setup.cfg
--rw-r--r--   0 adw0rd     (501) staff       (20)     1783 2023-05-22 11:37:03.000000 lamadava-1.0.7/setup.py
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-07-31 17:12:35.411797 lamadava-1.0.8/
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1072 2023-05-11 17:49:04.000000 lamadava-1.0.8/LICENSE
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1720 2023-07-31 17:12:35.411686 lamadava-1.0.8/PKG-INFO
+-rw-r--r--   0 adw0rd     (501) staff       (20)      670 2023-05-22 11:50:12.000000 lamadava-1.0.8/README.md
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-07-31 17:12:35.411020 lamadava-1.0.8/lamadava/
+-rw-r--r--   0 adw0rd     (501) staff       (20)      451 2023-06-05 21:44:38.000000 lamadava-1.0.8/lamadava/__init__.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)       96 2023-07-31 17:11:30.000000 lamadava-1.0.8/lamadava/__version__.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    30131 2023-07-31 17:10:42.000000 lamadava-1.0.8/lamadava/api.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)    31422 2023-07-31 17:10:42.000000 lamadava-1.0.8/lamadava/asyncapi.py
+-rw-r--r--   0 adw0rd     (501) staff       (20)     5829 2023-07-31 17:08:32.000000 lamadava-1.0.8/lamadava/base.py
+drwxr-xr-x   0 adw0rd     (501) staff       (20)        0 2023-07-31 17:12:35.411533 lamadava-1.0.8/lamadava.egg-info/
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1720 2023-07-31 17:12:35.000000 lamadava-1.0.8/lamadava.egg-info/PKG-INFO
+-rw-r--r--   0 adw0rd     (501) staff       (20)      284 2023-07-31 17:12:35.000000 lamadava-1.0.8/lamadava.egg-info/SOURCES.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)        1 2023-07-31 17:12:35.000000 lamadava-1.0.8/lamadava.egg-info/dependency_links.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)       14 2023-07-31 17:12:35.000000 lamadava-1.0.8/lamadava.egg-info/requires.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)        9 2023-07-31 17:12:35.000000 lamadava-1.0.8/lamadava.egg-info/top_level.txt
+-rw-r--r--   0 adw0rd     (501) staff       (20)       38 2023-07-31 17:12:35.411831 lamadava-1.0.8/setup.cfg
+-rw-r--r--   0 adw0rd     (501) staff       (20)     1783 2023-05-22 11:37:03.000000 lamadava-1.0.8/setup.py
```

### Comparing `lamadava-1.0.7/LICENSE` & `lamadava-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lamadava-1.0.7/PKG-INFO` & `lamadava-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamadava
-Version: 1.0.7
+Version: 1.0.8
 Summary: Lamadava client, for Python 3.
 Home-page: https://lamadava.com
 Author: Lamadava
 Author-email: support@lamadava.com
 License: MIT
 Keywords: instagram private api,instagram-private-api,instagram api,instagram-api,instagram,instagram-scraper,instagram-client,instagram-stories,instagram-feed,instagram-reels,instagram-insights,downloader,uploader,videos,photos,albums,igtv,reels,stories,pictures,instagram-user-photos,instagram-photos,instagram-metadata,instagram-downloader,instagram-uploader
 Classifier: Development Status :: 4 - Beta
```

### Comparing `lamadava-1.0.7/README.md` & `lamadava-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `lamadava-1.0.7/lamadava/api.py` & `lamadava-1.0.8/lamadava/api.py`

 * *Files identical despite different names*

### Comparing `lamadava-1.0.7/lamadava/asyncapi.py` & `lamadava-1.0.8/lamadava/asyncapi.py`

 * *Files identical despite different names*

### Comparing `lamadava-1.0.7/lamadava/base.py` & `lamadava-1.0.8/lamadava/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,17 @@
             method,
             url,
             headers=self._headers,
             params=params,
             data=data,
             timeout=self._timeout,
         )
-        return resp.json()
+        if "json" in resp.headers.get("content-type", "").lower():
+            return resp.json()
+        return resp.content
 
     def _paging_request(
         self,
         path: str,
         params: Optional[Dict[str, Any]],
         count: Optional[int] = None,
         container: Optional[List[Dict]] = None,
@@ -116,15 +118,17 @@
             method,
             url,
             headers=self._headers,
             params=params,
             data=data,
             timeout=self._timeout,
         )
-        return resp.json()
+        if "json" in resp.headers.get("content-type", "").lower():
+            return resp.json()
+        return resp.content
 
     async def _paging_request(
         self,
         path: str,
         params: Optional[Dict[str, Any]],
         count: Optional[int] = None,
         container: Optional[List[Dict]] = None,
```

### Comparing `lamadava-1.0.7/lamadava.egg-info/PKG-INFO` & `lamadava-1.0.8/lamadava.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamadava
-Version: 1.0.7
+Version: 1.0.8
 Summary: Lamadava client, for Python 3.
 Home-page: https://lamadava.com
 Author: Lamadava
 Author-email: support@lamadava.com
 License: MIT
 Keywords: instagram private api,instagram-private-api,instagram api,instagram-api,instagram,instagram-scraper,instagram-client,instagram-stories,instagram-feed,instagram-reels,instagram-insights,downloader,uploader,videos,photos,albums,igtv,reels,stories,pictures,instagram-user-photos,instagram-photos,instagram-metadata,instagram-downloader,instagram-uploader
 Classifier: Development Status :: 4 - Beta
```

### Comparing `lamadava-1.0.7/setup.py` & `lamadava-1.0.8/setup.py`

 * *Files identical despite different names*

