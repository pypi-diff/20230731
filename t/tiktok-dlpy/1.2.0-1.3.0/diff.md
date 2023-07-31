# Comparing `tmp/tiktok-dlpy-1.2.0.tar.gz` & `tmp/tiktok-dlpy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiktok-dlpy-1.2.0.tar", last modified: Thu Jul 20 15:26:47 2023, max compression
+gzip compressed data, was "tiktok-dlpy-1.3.0.tar", last modified: Mon Jul 31 20:40:00 2023, max compression
```

## Comparing `tiktok-dlpy-1.2.0.tar` & `tiktok-dlpy-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-07-20 15:26:47.782496 tiktok-dlpy-1.2.0/
--rw-r--r--   0 becky      (501) staff       (20)     1082 2023-05-26 11:18:26.000000 tiktok-dlpy-1.2.0/LICENSE
--rw-r--r--   0 becky      (501) staff       (20)      506 2023-07-20 15:26:47.782556 tiktok-dlpy-1.2.0/PKG-INFO
--rw-r--r--   0 becky      (501) staff       (20)      487 2023-06-12 14:02:52.000000 tiktok-dlpy-1.2.0/README.md
--rw-r--r--   0 becky      (501) staff       (20)       79 2023-07-20 15:26:47.782733 tiktok-dlpy-1.2.0/setup.cfg
--rw-r--r--   0 becky      (501) staff       (20)      766 2023-07-20 15:25:54.000000 tiktok-dlpy-1.2.0/setup.py
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-07-20 15:26:47.781441 tiktok-dlpy-1.2.0/tiktok_dlpy.egg-info/
--rw-r--r--   0 becky      (501) staff       (20)      506 2023-07-20 15:26:47.000000 tiktok-dlpy-1.2.0/tiktok_dlpy.egg-info/PKG-INFO
--rw-r--r--   0 becky      (501) staff       (20)      333 2023-07-20 15:26:47.000000 tiktok-dlpy-1.2.0/tiktok_dlpy.egg-info/SOURCES.txt
--rw-r--r--   0 becky      (501) staff       (20)        1 2023-07-20 15:26:47.000000 tiktok-dlpy-1.2.0/tiktok_dlpy.egg-info/dependency_links.txt
--rw-r--r--   0 becky      (501) staff       (20)       40 2023-07-20 15:26:47.000000 tiktok-dlpy-1.2.0/tiktok_dlpy.egg-info/requires.txt
--rw-r--r--   0 becky      (501) staff       (20)        9 2023-07-20 15:26:47.000000 tiktok-dlpy-1.2.0/tiktok_dlpy.egg-info/top_level.txt
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-07-20 15:26:47.782397 tiktok-dlpy-1.2.0/tiktokdl/
--rw-r--r--   0 becky      (501) staff       (20)       22 2023-05-27 18:10:11.000000 tiktok-dlpy-1.2.0/tiktokdl/__init__.py
--rw-r--r--   0 becky      (501) staff       (20)    13722 2023-07-20 15:24:21.000000 tiktok-dlpy-1.2.0/tiktokdl/download_video.py
--rw-r--r--   0 becky      (501) staff       (20)      434 2023-07-19 23:43:36.000000 tiktok-dlpy-1.2.0/tiktokdl/exceptions.py
--rw-r--r--   0 becky      (501) staff       (20)     2141 2023-05-26 12:21:24.000000 tiktok-dlpy-1.2.0/tiktokdl/image_processing.py
--rw-r--r--   0 becky      (501) staff       (20)      443 2023-06-11 17:49:11.000000 tiktok-dlpy-1.2.0/tiktokdl/video_data.py
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-07-31 20:40:00.183580 tiktok-dlpy-1.3.0/
+-rw-r--r--   0 becky      (501) staff       (20)     1082 2023-05-26 11:18:26.000000 tiktok-dlpy-1.3.0/LICENSE
+-rw-r--r--   0 becky      (501) staff       (20)      545 2023-07-31 20:40:00.183624 tiktok-dlpy-1.3.0/PKG-INFO
+-rw-r--r--   0 becky      (501) staff       (20)      539 2023-07-31 13:03:54.000000 tiktok-dlpy-1.3.0/README.md
+-rw-r--r--   0 becky      (501) staff       (20)       79 2023-07-31 20:40:00.183789 tiktok-dlpy-1.3.0/setup.cfg
+-rw-r--r--   0 becky      (501) staff       (20)      805 2023-07-31 13:03:49.000000 tiktok-dlpy-1.3.0/setup.py
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-07-31 20:40:00.182321 tiktok-dlpy-1.3.0/tiktok_dlpy.egg-info/
+-rw-r--r--   0 becky      (501) staff       (20)      545 2023-07-31 20:40:00.000000 tiktok-dlpy-1.3.0/tiktok_dlpy.egg-info/PKG-INFO
+-rw-r--r--   0 becky      (501) staff       (20)      331 2023-07-31 20:40:00.000000 tiktok-dlpy-1.3.0/tiktok_dlpy.egg-info/SOURCES.txt
+-rw-r--r--   0 becky      (501) staff       (20)        1 2023-07-31 20:40:00.000000 tiktok-dlpy-1.3.0/tiktok_dlpy.egg-info/dependency_links.txt
+-rw-r--r--   0 becky      (501) staff       (20)       40 2023-07-31 20:40:00.000000 tiktok-dlpy-1.3.0/tiktok_dlpy.egg-info/requires.txt
+-rw-r--r--   0 becky      (501) staff       (20)        9 2023-07-31 20:40:00.000000 tiktok-dlpy-1.3.0/tiktok_dlpy.egg-info/top_level.txt
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-07-31 20:40:00.183467 tiktok-dlpy-1.3.0/tiktokdl/
+-rw-r--r--   0 becky      (501) staff       (20)       22 2023-05-27 18:10:11.000000 tiktok-dlpy-1.3.0/tiktokdl/__init__.py
+-rw-r--r--   0 becky      (501) staff       (20)    14816 2023-07-31 13:00:18.000000 tiktok-dlpy-1.3.0/tiktokdl/download_post.py
+-rw-r--r--   0 becky      (501) staff       (20)      434 2023-07-19 23:43:36.000000 tiktok-dlpy-1.3.0/tiktokdl/exceptions.py
+-rw-r--r--   0 becky      (501) staff       (20)     2141 2023-05-26 12:21:24.000000 tiktok-dlpy-1.3.0/tiktokdl/image_processing.py
+-rw-r--r--   0 becky      (501) staff       (20)      560 2023-07-31 11:30:14.000000 tiktok-dlpy-1.3.0/tiktokdl/post_data.py
```

### Comparing `tiktok-dlpy-1.2.0/LICENSE` & `tiktok-dlpy-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tiktok-dlpy-1.2.0/setup.py` & `tiktok-dlpy-1.3.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tiktok-dlpy",
-    version="1.2.0",
+    version="1.3.0",
     url="https://github.com/Fluxticks/TikTokDL",
-    download_url="https://github.com/Fluxticks/TikTokDL/archive/v1.2.0.tar.gz",
+    download_url="https://github.com/Fluxticks/TikTokDL/archive/v1.3.0.tar.gz",
     author="Fluxticks",
     packages=find_packages(),
     install_requires=[
         "bs4",
         "lxml",
         "playwright",
         "numpy",
         "opencv-python",
     ],
-    description="A package to dowload TikTok videos via URL",
+    description="A package to download TikTok videos or slideshows by URL without needing to login",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10"
     ],
     keywords=["tiktok",
```

### Comparing `tiktok-dlpy-1.2.0/tiktokdl/download_video.py` & `tiktok-dlpy-1.3.0/tiktokdl/download_post.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import inspect
 import json
 from datetime import datetime
 import random
 import time
 from typing import Literal
 from urllib.parse import parse_qs, urlparse
+from urllib.request import urlretrieve
 
 from bs4 import BeautifulSoup
 from playwright.async_api import Error as PlaywrightError
 from playwright.async_api import Page, Request, BrowserContext
 from playwright.async_api import TimeoutError as PlaywrightTimeoutError
 from playwright.async_api import async_playwright
 
 from tiktokdl.exceptions import CaptchaFailedException, DownloadFailedException, ResponseParseException
 from tiktokdl.image_processing import find_position, image_from_url
-from tiktokdl.video_data import TikTokVideo
+from tiktokdl.post_data import TikTokVideo, TikTokSlide, TikTokPost
 
-__all__ = ["get_video"]
+__all__ = ["get_post"]
 
 
 def __parse_captcha_params_from_url(url: str) -> dict:
     parsed_url = urlparse(url, allow_fragments=False)
     params = parse_qs(parsed_url.query)
     out = {}
     for key, value in params.items():
@@ -36,55 +37,71 @@
 
 async def __get_captcha_response_headers(request: Request) -> dict:
     all_headers = await request.all_headers()
     all_headers["content-type"] = "application/json;charset=UTF-8"
     return all_headers
 
 
-def __parse_video_info(page_source: str) -> TikTokVideo:
+def __is_image_post(post_data: dict) -> bool:
+    return post_data.get("imagePost") is not None
+
+
+def __parse_post_info(page_source: str) -> TikTokVideo | TikTokSlide:
     soup = BeautifulSoup(page_source, "lxml")
     script_data = soup.find("script", attrs={"id": "SIGI_STATE"})
     data = json.loads(script_data.text)
 
     post_url = data.get("SEOState").get("canonical")
 
     author_data = list(data.get("UserModule").get("users").values())[0]
     username = author_data.get("uniqueId")
     display_name = author_data.get("nickname")
     avatar = author_data.get("avatarThumb")
     author_url = f"https://www.tiktok.com/@{username}/"
 
-    video_data = list(data.get("ItemModule").values())[0]
-    video_description = video_data.get("desc")
-    video_download_setting = video_data.get("downloadSetting")
-    video_id = video_data.get("id")
-    timestamp = datetime.fromtimestamp(int(video_data.get("createTime")))
-    like_count = video_data.get("stats").get("diggCount")
-    share_count = video_data.get("stats").get("shareCount")
-    comment_count = video_data.get("stats").get("commentCount")
-    view_count = video_data.get("stats").get("playCount")
-    video_thumbnail = video_data.get("video").get("originCover")
-
-    return TikTokVideo(
-        url=post_url,
-        video_id=video_id,
-        author_username=username,
-        author_display_name=display_name,
-        author_avatar=avatar,
-        author_url=author_url,
-        video_download_setting=video_download_setting,
-        video_description=video_description,
-        timestamp=timestamp,
-        like_count=like_count,
-        share_count=share_count,
-        comment_count=comment_count,
-        view_count=view_count,
-        video_thumbnail=video_thumbnail,
+    post_data = list(data.get("ItemModule").values())[0]
+
+    post_description = post_data.get("desc")
+    post_download_setting = post_data.get("downloadSetting")
+    post_id = post_data.get("id")
+    timestamp = datetime.fromtimestamp(int(post_data.get("createTime")))
+    like_count = post_data.get("stats").get("diggCount")
+    share_count = post_data.get("stats").get("shareCount")
+    comment_count = post_data.get("stats").get("commentCount")
+    view_count = post_data.get("stats").get("playCount")
+
+    post = TikTokPost(
+            url=post_url,
+            post_id=post_id,
+            author_username=username,
+            author_display_name=display_name,
+            author_avatar=avatar,
+            author_url=author_url,
+            post_download_setting=post_download_setting,
+            post_description=post_description,
+            timestamp=timestamp,
+            like_count=like_count,
+            share_count=share_count,
+            comment_count=comment_count,
+            view_count=view_count
     )
 
+    if __is_image_post(post_data):
+        images = post_data.get("imagePost").get("images")
+        return TikTokSlide(
+            **post.__dict__,
+            images=images
+        )
+    else:
+        video_thumbnail = post_data.get("video").get("originCover")
+        return TikTokVideo(
+             **post.__dict__,
+            video_thumbnail=video_thumbnail
+        )
+
 
 def __generate_random_captcha_steps(piece_position: tuple[int, int], tip_y_value: int):
     x_position = piece_position[0]
 
     steps = []
     current_distance = 0
     relative_time = random.randint(100, 300)
@@ -187,30 +204,30 @@
     for key, value in all_kwargs.items():
         if key in allowed_args:
             valid_kwargs[key] = value
 
     return valid_kwargs
 
 
-async def get_video(
+async def get_post(
     url: str,
     download: bool = True,
     force_download_strategy: Literal["primary",
                                      "secondary"] | None = None,
     proxy: dict | None = None,
     download_timeout: float = 5000,
     browser: Literal["firefox",
                      "chromium",
                      "chrome",
                      "safari",
                      "webkit"] = "firefox",
     headless: bool | None = None,
     slow_mo: float | None = None,
     **kwargs: dict
-) -> TikTokVideo:
+) -> TikTokVideo | TikTokSlide:
     """Get the information about a given video URL. If the `download` param is set to True, also download the video as an mp4 file.
 
     Args:
         url (str): The URL to get the information of.
         download (bool, optional): If the video should be downloaded locally. Defaults to True.
         force_download_strategy (Literal[&quot;primary&quot;, &quot;secondary&quot;] | None, optional): Force a specific download strategy to use. Defaults to None which will auto-select the strategy to use.
         proxy (dict | None, optional): The proxy settings to use for the request. Defaults to None.
@@ -251,27 +268,31 @@
         await browser_context.clear_cookies()
 
         video_page = await browser_context.new_page()
         await video_page.goto(url)
 
         try:
             page_source = await video_page.content()
-            video_info = __parse_video_info(page_source)
+            video_info = __parse_post_info(page_source)
         except:
             raise ResponseParseException(url)
 
         if not download:
             return video_info
 
         captcha_success_result = await __handle_captcha(video_page)
         if not captcha_success_result:
             raise CaptchaFailedException(url)
 
         await __close_popups(video_page)
 
+        if isinstance(video_info, TikTokSlide):
+            await download_slideshow(video_info)
+            return video_info
+
         if force_download_strategy:
             try:
                 match force_download_strategy:
                     case "primary":
                         await primary_download_strategy(browser_context, video_page, video_info, download_timeout)
                     case "secondary":
                         await alternate_download_strategy(video_page, video_info, download_timeout)
@@ -337,7 +358,23 @@
     async with playwright_page.expect_response(lambda x: response_base_url in x.url, timeout=timeout) as response_info:
         await playwright_page.reload()
         response = await response_info.value
         save_path = f"{video_info.video_id}.mp4"
         with open(save_path, "wb") as f:
             f.write(await response.body())
         video_info.file_path = save_path
+
+
+async def download_slideshow(video_info: TikTokSlide):
+    """For a given Slideshow post, download the images associated with it.
+
+    Args:
+        video_info (TikTokSlide): The Slideshow post data.
+    """
+    images = []
+    for idx, image_info in enumerate(video_info.images):
+        image_url = image_info.get("imageURL").get("urlList")[-1]
+        file = f"{idx+1}.jpeg"
+        urlretrieve(image_url, file)
+        images.append(file)
+
+    video_info.images = images
```

### Comparing `tiktok-dlpy-1.2.0/tiktokdl/image_processing.py` & `tiktok-dlpy-1.3.0/tiktokdl/image_processing.py`

 * *Files identical despite different names*

