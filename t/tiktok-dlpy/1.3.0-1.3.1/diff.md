# Comparing `tmp/tiktok-dlpy-1.3.0.tar.gz` & `tmp/tiktok-dlpy-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiktok-dlpy-1.3.0.tar", last modified: Mon Jul 31 20:40:00 2023, max compression
+gzip compressed data, was "tiktok-dlpy-1.3.1.tar", last modified: Mon Jul 31 21:45:39 2023, max compression
```

## Comparing `tiktok-dlpy-1.3.0.tar` & `tiktok-dlpy-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-07-31 20:40:00.183580 tiktok-dlpy-1.3.0/
--rw-r--r--   0 becky      (501) staff       (20)     1082 2023-05-26 11:18:26.000000 tiktok-dlpy-1.3.0/LICENSE
--rw-r--r--   0 becky      (501) staff       (20)      545 2023-07-31 20:40:00.183624 tiktok-dlpy-1.3.0/PKG-INFO
--rw-r--r--   0 becky      (501) staff       (20)      539 2023-07-31 13:03:54.000000 tiktok-dlpy-1.3.0/README.md
--rw-r--r--   0 becky      (501) staff       (20)       79 2023-07-31 20:40:00.183789 tiktok-dlpy-1.3.0/setup.cfg
--rw-r--r--   0 becky      (501) staff       (20)      805 2023-07-31 13:03:49.000000 tiktok-dlpy-1.3.0/setup.py
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-07-31 20:40:00.182321 tiktok-dlpy-1.3.0/tiktok_dlpy.egg-info/
--rw-r--r--   0 becky      (501) staff       (20)      545 2023-07-31 20:40:00.000000 tiktok-dlpy-1.3.0/tiktok_dlpy.egg-info/PKG-INFO
--rw-r--r--   0 becky      (501) staff       (20)      331 2023-07-31 20:40:00.000000 tiktok-dlpy-1.3.0/tiktok_dlpy.egg-info/SOURCES.txt
--rw-r--r--   0 becky      (501) staff       (20)        1 2023-07-31 20:40:00.000000 tiktok-dlpy-1.3.0/tiktok_dlpy.egg-info/dependency_links.txt
--rw-r--r--   0 becky      (501) staff       (20)       40 2023-07-31 20:40:00.000000 tiktok-dlpy-1.3.0/tiktok_dlpy.egg-info/requires.txt
--rw-r--r--   0 becky      (501) staff       (20)        9 2023-07-31 20:40:00.000000 tiktok-dlpy-1.3.0/tiktok_dlpy.egg-info/top_level.txt
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-07-31 20:40:00.183467 tiktok-dlpy-1.3.0/tiktokdl/
--rw-r--r--   0 becky      (501) staff       (20)       22 2023-05-27 18:10:11.000000 tiktok-dlpy-1.3.0/tiktokdl/__init__.py
--rw-r--r--   0 becky      (501) staff       (20)    14816 2023-07-31 13:00:18.000000 tiktok-dlpy-1.3.0/tiktokdl/download_post.py
--rw-r--r--   0 becky      (501) staff       (20)      434 2023-07-19 23:43:36.000000 tiktok-dlpy-1.3.0/tiktokdl/exceptions.py
--rw-r--r--   0 becky      (501) staff       (20)     2141 2023-05-26 12:21:24.000000 tiktok-dlpy-1.3.0/tiktokdl/image_processing.py
--rw-r--r--   0 becky      (501) staff       (20)      560 2023-07-31 11:30:14.000000 tiktok-dlpy-1.3.0/tiktokdl/post_data.py
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-07-31 21:45:39.106501 tiktok-dlpy-1.3.1/
+-rw-r--r--   0 becky      (501) staff       (20)     1082 2023-05-26 11:18:26.000000 tiktok-dlpy-1.3.1/LICENSE
+-rw-r--r--   0 becky      (501) staff       (20)      545 2023-07-31 21:45:39.106554 tiktok-dlpy-1.3.1/PKG-INFO
+-rw-r--r--   0 becky      (501) staff       (20)      539 2023-07-31 21:43:57.000000 tiktok-dlpy-1.3.1/README.md
+-rw-r--r--   0 becky      (501) staff       (20)       79 2023-07-31 21:45:39.106751 tiktok-dlpy-1.3.1/setup.cfg
+-rw-r--r--   0 becky      (501) staff       (20)      805 2023-07-31 21:44:43.000000 tiktok-dlpy-1.3.1/setup.py
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-07-31 21:45:39.105862 tiktok-dlpy-1.3.1/tiktok_dlpy.egg-info/
+-rw-r--r--   0 becky      (501) staff       (20)      545 2023-07-31 21:45:39.000000 tiktok-dlpy-1.3.1/tiktok_dlpy.egg-info/PKG-INFO
+-rw-r--r--   0 becky      (501) staff       (20)      331 2023-07-31 21:45:39.000000 tiktok-dlpy-1.3.1/tiktok_dlpy.egg-info/SOURCES.txt
+-rw-r--r--   0 becky      (501) staff       (20)        1 2023-07-31 21:45:39.000000 tiktok-dlpy-1.3.1/tiktok_dlpy.egg-info/dependency_links.txt
+-rw-r--r--   0 becky      (501) staff       (20)       40 2023-07-31 21:45:39.000000 tiktok-dlpy-1.3.1/tiktok_dlpy.egg-info/requires.txt
+-rw-r--r--   0 becky      (501) staff       (20)        9 2023-07-31 21:45:39.000000 tiktok-dlpy-1.3.1/tiktok_dlpy.egg-info/top_level.txt
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-07-31 21:45:39.106411 tiktok-dlpy-1.3.1/tiktokdl/
+-rw-r--r--   0 becky      (501) staff       (20)       22 2023-05-27 18:10:11.000000 tiktok-dlpy-1.3.1/tiktokdl/__init__.py
+-rw-r--r--   0 becky      (501) staff       (20)    14813 2023-07-31 21:44:03.000000 tiktok-dlpy-1.3.1/tiktokdl/download_post.py
+-rw-r--r--   0 becky      (501) staff       (20)      434 2023-07-19 23:43:36.000000 tiktok-dlpy-1.3.1/tiktokdl/exceptions.py
+-rw-r--r--   0 becky      (501) staff       (20)     2141 2023-05-26 12:21:24.000000 tiktok-dlpy-1.3.1/tiktokdl/image_processing.py
+-rw-r--r--   0 becky      (501) staff       (20)      560 2023-07-31 21:43:57.000000 tiktok-dlpy-1.3.1/tiktokdl/post_data.py
```

### Comparing `tiktok-dlpy-1.3.0/LICENSE` & `tiktok-dlpy-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tiktok-dlpy-1.3.0/PKG-INFO` & `tiktok-dlpy-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tiktok-dlpy
-Version: 1.3.0
+Version: 1.3.1
 Summary: A package to download TikTok videos or slideshows by URL without needing to login
 Home-page: https://github.com/Fluxticks/TikTokDL
-Download-URL: https://github.com/Fluxticks/TikTokDL/archive/v1.3.0.tar.gz
+Download-URL: https://github.com/Fluxticks/TikTokDL/archive/v1.3.1.tar.gz
 Author: Fluxticks
 Keywords: tiktok,playwright,async
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
```

### Comparing `tiktok-dlpy-1.3.0/README.md` & `tiktok-dlpy-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tiktok-dlpy-1.3.0/setup.py` & `tiktok-dlpy-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tiktok-dlpy",
-    version="1.3.0",
+    version="1.3.1",
     url="https://github.com/Fluxticks/TikTokDL",
-    download_url="https://github.com/Fluxticks/TikTokDL/archive/v1.3.0.tar.gz",
+    download_url="https://github.com/Fluxticks/TikTokDL/archive/v1.3.1.tar.gz",
     author="Fluxticks",
     packages=find_packages(),
     install_requires=[
         "bs4",
         "lxml",
         "playwright",
         "numpy",
```

### Comparing `tiktok-dlpy-1.3.0/tiktok_dlpy.egg-info/PKG-INFO` & `tiktok-dlpy-1.3.1/tiktok_dlpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tiktok-dlpy
-Version: 1.3.0
+Version: 1.3.1
 Summary: A package to download TikTok videos or slideshows by URL without needing to login
 Home-page: https://github.com/Fluxticks/TikTokDL
-Download-URL: https://github.com/Fluxticks/TikTokDL/archive/v1.3.0.tar.gz
+Download-URL: https://github.com/Fluxticks/TikTokDL/archive/v1.3.1.tar.gz
 Author: Fluxticks
 Keywords: tiktok,playwright,async
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
```

### Comparing `tiktok-dlpy-1.3.0/tiktokdl/download_post.py` & `tiktok-dlpy-1.3.1/tiktokdl/download_post.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,15 @@
                         )
             except:
                 raise DownloadFailedException(url=url)
 
             return video_info
 
         try:
-            if video_info.video_download_setting == 0:
+            if video_info.post_download_setting == 0:
                 await primary_download_strategy(browser_context, video_page, video_info, download_timeout)
             else:
                 await alternate_download_strategy(video_page, video_info, download_timeout)
         except PlaywrightTimeoutError:
             raise DownloadFailedException(url=url)
 
         return video_info
@@ -334,15 +334,15 @@
     page_video_tag = playwright_page.locator("video").first
     await page_video_tag.click(button="right")
     await __random_timeout_duration(playwright_page, 100, 500)
     download_video_li = playwright_page.locator("li", has_text="Download video")
     async with playwright_page.expect_download() as download_info:
         await download_video_li.click()
         download = await download_info.value
-        save_path = f"{video_info.video_id}.mp4"
+        save_path = f"{video_info.post_id}.mp4"
         await download.save_as(save_path)
         video_info.file_path = save_path
 
 
 async def alternate_download_strategy(playwright_page: Page, video_info: TikTokVideo, timeout: float):
     """Uses the the browser request for the video to download the video. Valid for any download setting but less reliable.
 
@@ -354,15 +354,15 @@
     page_video_tag = playwright_page.locator("video").first
     video_source = await page_video_tag.get_attribute("src")
 
     response_base_url = video_source.split("?")[0]
     async with playwright_page.expect_response(lambda x: response_base_url in x.url, timeout=timeout) as response_info:
         await playwright_page.reload()
         response = await response_info.value
-        save_path = f"{video_info.video_id}.mp4"
+        save_path = f"{video_info.post_id}.mp4"
         with open(save_path, "wb") as f:
             f.write(await response.body())
         video_info.file_path = save_path
 
 
 async def download_slideshow(video_info: TikTokSlide):
     """For a given Slideshow post, download the images associated with it.
```

### Comparing `tiktok-dlpy-1.3.0/tiktokdl/image_processing.py` & `tiktok-dlpy-1.3.1/tiktokdl/image_processing.py`

 * *Files identical despite different names*

### Comparing `tiktok-dlpy-1.3.0/tiktokdl/post_data.py` & `tiktok-dlpy-1.3.1/tiktokdl/post_data.py`

 * *Files identical despite different names*

