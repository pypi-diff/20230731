# Comparing `tmp/jmcomic-2.1.5.tar.gz` & `tmp/jmcomic-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jmcomic-2.1.5.tar", last modified: Wed Jul 26 09:44:12 2023, max compression
+gzip compressed data, was "jmcomic-2.1.6.tar", last modified: Mon Jul 31 05:53:01 2023, max compression
```

## Comparing `jmcomic-2.1.5.tar` & `jmcomic-2.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:44:12.644325 jmcomic-2.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-26 09:44:01.000000 jmcomic-2.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-26 09:44:12.644325 jmcomic-2.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-26 09:44:01.000000 jmcomic-2.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 09:44:12.644325 jmcomic-2.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-26 09:44:01.000000 jmcomic-2.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:44:12.640325 jmcomic-2.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:44:12.644325 jmcomic-2.1.5/src/jmcomic/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-26 09:44:01.000000 jmcomic-2.1.5/src/jmcomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-26 09:44:01.000000 jmcomic-2.1.5/src/jmcomic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-07-26 09:44:01.000000 jmcomic-2.1.5/src/jmcomic/jm_client_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-07-26 09:44:01.000000 jmcomic-2.1.5/src/jmcomic/jm_client_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-26 09:44:01.000000 jmcomic-2.1.5/src/jmcomic/jm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-07-26 09:44:01.000000 jmcomic-2.1.5/src/jmcomic/jm_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-07-26 09:44:01.000000 jmcomic-2.1.5/src/jmcomic/jm_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-07-26 09:44:01.000000 jmcomic-2.1.5/src/jmcomic/jm_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:44:12.644325 jmcomic-2.1.5/src/jmcomic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-26 09:44:12.000000 jmcomic-2.1.5/src/jmcomic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-26 09:44:12.000000 jmcomic-2.1.5/src/jmcomic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 09:44:12.000000 jmcomic-2.1.5/src/jmcomic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-26 09:44:12.000000 jmcomic-2.1.5/src/jmcomic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 09:44:12.000000 jmcomic-2.1.5/src/jmcomic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:53:01.701327 jmcomic-2.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 05:52:47.000000 jmcomic-2.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-31 05:53:01.701327 jmcomic-2.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-31 05:52:47.000000 jmcomic-2.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 05:53:01.701327 jmcomic-2.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-31 05:52:47.000000 jmcomic-2.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:53:01.697327 jmcomic-2.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:53:01.701327 jmcomic-2.1.6/src/jmcomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 05:52:47.000000 jmcomic-2.1.6/src/jmcomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-31 05:52:47.000000 jmcomic-2.1.6/src/jmcomic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-07-31 05:52:47.000000 jmcomic-2.1.6/src/jmcomic/jm_client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-07-31 05:52:47.000000 jmcomic-2.1.6/src/jmcomic/jm_client_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-07-31 05:52:47.000000 jmcomic-2.1.6/src/jmcomic/jm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-07-31 05:52:47.000000 jmcomic-2.1.6/src/jmcomic/jm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-07-31 05:52:47.000000 jmcomic-2.1.6/src/jmcomic/jm_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-07-31 05:52:47.000000 jmcomic-2.1.6/src/jmcomic/jm_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 05:53:01.701327 jmcomic-2.1.6/src/jmcomic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-31 05:53:01.000000 jmcomic-2.1.6/src/jmcomic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-31 05:53:01.000000 jmcomic-2.1.6/src/jmcomic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 05:53:01.000000 jmcomic-2.1.6/src/jmcomic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 05:53:01.000000 jmcomic-2.1.6/src/jmcomic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 05:53:01.000000 jmcomic-2.1.6/src/jmcomic.egg-info/top_level.txt
```

### Comparing `jmcomic-2.1.5/LICENSE` & `jmcomic-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.5/PKG-INFO` & `jmcomic-2.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.1.5
+Version: 2.1.6
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -39,43 +39,48 @@
 
   ```shell
   pip install -e ./
   ```
 
 ## 快速上手
 
-使用下面的两行代码，即可实现功能：把某个本子集（album）里的所有本子（photo）下载到本地
+使用下面的两行代码，即可实现功能：把某个本子（album）里的所有章节（photo）下载到本地
 
 ```python
 import jmcomic  # 导入此模块，需要先安装.
 jmcomic.download_album('422866')  # 传入要下载的album的id，即可下载整个album到本地.
 # 上面的这行代码，还有一个可选参数option: JmOption，表示配置项，
 # 配置项的作用是告诉程序下载时候的一些选择，
-# 比如，要下载到哪个文件夹，使用怎样的路径组织方式（比如[/作者/本子id/图片] 或者 [/作者/本子名称/图片]）.
+# 比如，要下载到哪个文件夹，使用怎样的路径组织规则（比如[/作者/本子id/图片] 或者 [/作者/本子名称/图片]）.
 # 如果没有配置，则会使用 JmOption.default()，下载的路径是[当前工作文件夹/本子名称/图片].
+# 如果你想要配置，请参考assets/config/和usgae/下的文档和示例.
 ```
 
 进一步的使用可以参考usage文件夹下的示例代码: `getting_started.py` `sample_usage.py`
 
 ## 项目特点
 
 - **绕过Cloudflare的反爬虫**
 - 支持使用**Github Action**下载漫画，不会编程都能用（[教程：使用Github Actions下载禁漫本子](./assets/docs/教程：使用Github%20Actions下载禁漫本子.md)）
 - 可配置性强
-
   - 不配置也能使用，十分方便
-  - 配置可以从**配置文件**生成，无需写Python代码
-  - 配置点有：`是否使用磁盘缓存`  `是否使用代理` `图片类型转换` `本子下载路径` `请求元信息（headers,cookies,重试次数）等 `
+  - 配置可以从**配置文件**生成，支持多种文件格式，无需写Python代码
+  - 配置点有：`是否使用磁盘缓存` `图片类型转换` `下载路径` `请求元信息（headers,cookies,代理）等 `
+- 可扩展性强
+  - 支持自定义本子/章节/图片下载前后的回调函数
+  - 支持自定义debug日志的开关/格式
+  - 支持自定义Option/Client/实体类
+- 支持重试和域名切换机制
 - 多线程下载（可细化到一图一线程，效率极高）
 - 跟进了JM最新的图片分割算法（2023-02-08）
 
 ## 使用小说明
 
 * Python >= 3.7
-* 项目只有代码注释，没有API文档。因此想深入高级地使用，自行看源码和改造代码叭 ^^_
+* 个人项目，文档和示例会有不及时之处，可以Issue提问
 
 ## 项目文件夹介绍
 
 * assets：存放一些非代码的资源文件
 
   * config：存放配置文件
   * docs：项目文档
```

### Comparing `jmcomic-2.1.5/README.md` & `jmcomic-2.1.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,43 +17,48 @@
 
   ```shell
   pip install -e ./
   ```
 
 ## 快速上手
 
-使用下面的两行代码，即可实现功能：把某个本子集（album）里的所有本子（photo）下载到本地
+使用下面的两行代码，即可实现功能：把某个本子（album）里的所有章节（photo）下载到本地
 
 ```python
 import jmcomic  # 导入此模块，需要先安装.
 jmcomic.download_album('422866')  # 传入要下载的album的id，即可下载整个album到本地.
 # 上面的这行代码，还有一个可选参数option: JmOption，表示配置项，
 # 配置项的作用是告诉程序下载时候的一些选择，
-# 比如，要下载到哪个文件夹，使用怎样的路径组织方式（比如[/作者/本子id/图片] 或者 [/作者/本子名称/图片]）.
+# 比如，要下载到哪个文件夹，使用怎样的路径组织规则（比如[/作者/本子id/图片] 或者 [/作者/本子名称/图片]）.
 # 如果没有配置，则会使用 JmOption.default()，下载的路径是[当前工作文件夹/本子名称/图片].
+# 如果你想要配置，请参考assets/config/和usgae/下的文档和示例.
 ```
 
 进一步的使用可以参考usage文件夹下的示例代码: `getting_started.py` `sample_usage.py`
 
 ## 项目特点
 
 - **绕过Cloudflare的反爬虫**
 - 支持使用**Github Action**下载漫画，不会编程都能用（[教程：使用Github Actions下载禁漫本子](./assets/docs/教程：使用Github%20Actions下载禁漫本子.md)）
 - 可配置性强
-
   - 不配置也能使用，十分方便
-  - 配置可以从**配置文件**生成，无需写Python代码
-  - 配置点有：`是否使用磁盘缓存`  `是否使用代理` `图片类型转换` `本子下载路径` `请求元信息（headers,cookies,重试次数）等 `
+  - 配置可以从**配置文件**生成，支持多种文件格式，无需写Python代码
+  - 配置点有：`是否使用磁盘缓存` `图片类型转换` `下载路径` `请求元信息（headers,cookies,代理）等 `
+- 可扩展性强
+  - 支持自定义本子/章节/图片下载前后的回调函数
+  - 支持自定义debug日志的开关/格式
+  - 支持自定义Option/Client/实体类
+- 支持重试和域名切换机制
 - 多线程下载（可细化到一图一线程，效率极高）
 - 跟进了JM最新的图片分割算法（2023-02-08）
 
 ## 使用小说明
 
 * Python >= 3.7
-* 项目只有代码注释，没有API文档。因此想深入高级地使用，自行看源码和改造代码叭 ^^_
+* 个人项目，文档和示例会有不及时之处，可以Issue提问
 
 ## 项目文件夹介绍
 
 * assets：存放一些非代码的资源文件
 
   * config：存放配置文件
   * docs：项目文档
```

### Comparing `jmcomic-2.1.5/setup.py` & `jmcomic-2.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.5/src/jmcomic/api.py` & `jmcomic-2.1.6/src/jmcomic/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         return download_album_batch(jm_album_id, option)
 
     option, jm_client = build_client(option)
     album: JmAlbumDetail = jm_client.get_album_detail(jm_album_id)
 
     option.before_album(album)
     execute_by_condition(
-        iter_obj=album,
+        iter_objs=album,
         apply=lambda photo: download_by_photo_detail(photo, option),
         count_batch=option.decide_photo_batch_count(album)
     )
     option.after_album(album)
 
 
 def download_photo(jm_photo_id, option=None):
@@ -45,31 +45,29 @@
     use_cache = option.download_cache
     decode_image = option.download_image_decode
     jm_client.check_photo(photo)
 
     # 下载每个图片的函数
     def download_image(image: JmImageDetail):
         img_save_path = option.decide_image_filepath(image)
-
-        # 已下载过，缓存命中
-        if use_cache is True and file_exists(img_save_path):
-            image.is_exists = True
-            return
+        image.is_exists = file_exists(img_save_path)
 
         option.before_image(image, img_save_path)
+        if use_cache is True and image.is_exists:
+            return
         jm_client.download_by_image_detail(
             image,
             img_save_path,
             decode_image=decode_image,
         )
         option.after_image(image, img_save_path)
 
     option.before_photo(photo)
     execute_by_condition(
-        iter_obj=photo,
+        iter_objs=photo,
         apply=download_image,
         count_batch=option.decide_image_batch_count(photo)
     )
     option.before_photo(photo)
 
 
 def download_album_batch(jm_album_id_iter: Union[Iterable, Generator],
@@ -84,36 +82,36 @@
     @param wait_finish: 是否要等待这些下载线程全部完成
     @return 返回值是List[Thread]，里面是每个下载漫画的线程。
     """
     if option is None:
         option = JmOption.default()
 
     return thread_pool_executor(
-        iter_objs=((album_id, option) for album_id in jm_album_id_iter),
-        apply_each_obj_func=download_album,
+        iter_objs=set(JmcomicText.parse_to_album_id(album_id) for album_id in jm_album_id_iter),
+        apply_each_obj_func=lambda album_id: download_album(album_id, option),
         wait_finish=wait_finish,
     )
 
 
-def execute_by_condition(iter_obj, apply: Callable, count_batch: int):
+def execute_by_condition(iter_objs, apply: Callable, count_batch: int):
     """
     章节/图片的下载调度逻辑
     """
-    count_real = len(iter_obj)
+    count_real = len(iter_objs)
 
     if count_batch >= count_real:
-        # 一图一线程
+        # 一个图/章节 对应 一个线程
         multi_thread_launcher(
-            iter_objs=iter_obj,
+            iter_objs=iter_objs,
             apply_each_obj_func=apply,
         )
     else:
-        # 创建batch个线程的线程池，当图片数>batch时要等待。
+        # 创建batch个线程的线程池
         thread_pool_executor(
-            iter_objs=iter_obj,
+            iter_objs=iter_objs,
             apply_each_obj_func=apply,
             max_workers=count_batch,
         )
 
 
 def build_client(option: Optional[JmOption]) -> Tuple[JmOption, JmcomicClient]:
     """
```

### Comparing `jmcomic-2.1.5/src/jmcomic/jm_client_impl.py` & `jmcomic-2.1.6/src/jmcomic/jm_client_impl.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.5/src/jmcomic/jm_client_interface.py` & `jmcomic-2.1.6/src/jmcomic/jm_client_interface.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.5/src/jmcomic/jm_config.py` & `jmcomic-2.1.6/src/jmcomic/jm_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+def field_cache(*args, **kwargs):
+    from common import field_cache
+    return field_cache(*args, **kwargs)
+
+
 def default_jm_debug(topic: str, msg: str):
     from common import format_ts
     print(f'{format_ts()}:【{topic}】{msg}')
 
 
 def default_postman_constructor(session, **kwargs):
     from common import Postmans
@@ -11,19 +16,21 @@
 
     return Postmans.new_postman(**kwargs)
 
 
 class JmModuleConfig:
     # 网站相关
     PROT = "https://"
-    DOMAIN = None
     JM_REDIRECT_URL = f'{PROT}jm365.work/3YeBdF'  # 永久網域，怕走失的小伙伴收藏起来
     JM_PUB_URL = f'{PROT}jmcomic2.bet'
     JM_CDN_IMAGE_URL_TEMPLATE = PROT + 'cdn-msp.{domain}/media/photos/{photo_id}/{index:05}{suffix}'  # index 从1开始
     JM_IMAGE_SUFFIX = ['.jpg', '.webp', '.png', '.gif']
+    # 缓存字段
+    DOMAIN = None
+    DOMAIN_LIST = None
 
     # 访问JM可能会遇到的异常网页
     JM_ERROR_RESPONSE_TEXT = {
         "Could not connect to mysql! Please check your database settings!": "禁漫服务器内部报错",
         "Restricted Access!": "禁漫拒绝你所在ip地区的访问，你可以选择: 换域名/换代理",
     }
 
@@ -48,25 +55,23 @@
 
     # debug
     enable_jm_debug = True
     debug_executor = default_jm_debug
     postman_constructor = default_postman_constructor
 
     @classmethod
+    @field_cache("DOMAIN")
     def domain(cls, postman=None):
         """
         由于禁漫的域名经常变化，调用此方法可以获取一个当前可用的最新的域名 domain，
         并且设置把 domain 设置为禁漫模块的默认域名。
         这样一来，配置文件也不用配置域名了，一切都在运行时动态获取。
         """
-        if cls.DOMAIN is None:
-            from .jm_toolkit import JmcomicText
-            cls.DOMAIN = JmcomicText.parse_to_jm_domain(cls.get_jmcomic_url(postman))
-
-        return cls.DOMAIN  # jmcomic默认域名
+        from .jm_toolkit import JmcomicText
+        return JmcomicText.parse_to_jm_domain(cls.get_jmcomic_url(postman))
 
     @classmethod
     def headers(cls, domain='18comic.vip'):
         return {
             'authority': domain,
             'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,'
                       'application/signed-exchange;v=b3;q=0.7',
@@ -112,14 +117,15 @@
 
         resp = postman.get(cls.JM_REDIRECT_URL)
         url = resp.url
         cls.jm_debug('获取禁漫地址', f'[{cls.JM_REDIRECT_URL}] → [{url}]')
         return url
 
     @classmethod
+    @field_cache("DOMAIN_LIST")
     def get_jmcomic_domain_all(cls, postman=None):
         """
         访问禁漫发布页，得到所有禁漫的域名
         @return：['18comic.vip', ..., 'jm365.xyz/ZNPJam'], 最后一个是【APP軟件下載】
         """
         postman = postman or cls.new_postman(session=True)
```

### Comparing `jmcomic-2.1.5/src/jmcomic/jm_entity.py` & `jmcomic-2.1.6/src/jmcomic/jm_entity.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.5/src/jmcomic/jm_option.py` & `jmcomic-2.1.6/src/jmcomic/jm_option.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     def before_image(self, image: JmImageDetail, img_save_path):
         if image.is_exists:
             jm_debug('image-before',
                      f'图片已存在: {image.tag} ← [{img_save_path}]'
                      )
         else:
-            jm_debug('image_before',
+            jm_debug('image-before',
                      f'图片准备下载: {image.tag}, [{image.img_url}] → [{img_save_path}]'
                      )
 
     def after_image(self, image: JmImageDetail, img_save_path):
         jm_debug('image-after',
                  f'图片下载完成: {image.tag}, [{image.img_url}] → [{img_save_path}]')
 
@@ -155,17 +155,14 @@
         # 请求配置
         self.client = DictModel(client)
         # 下载配置
         self.download = DictModel(download)
         # 其他配置
         self.filepath = filepath
 
-        # 字段
-        self.jm_client_cache = None
-
     @property
     def download_cache(self):
         return self.download.cache
 
     @property
     def download_image_decode(self):
         return self.download.image.decode
@@ -182,17 +179,17 @@
     下面是决定图片保存路径的方法
     """
 
     # noinspection PyUnusedLocal
     def decide_image_batch_count(self, photo: JmPhotoDetail):
         return self.download_threading_batch_count
 
-    # noinspection PyMethodMayBeStatic
+    # noinspection PyMethodMayBeStatic,PyUnusedLocal
     def decide_photo_batch_count(self, album: JmAlbumDetail):
-        return len(album)
+        return os.cpu_count()
 
     def decide_image_save_dir(self, photo) -> str:
         # 使用 self.dir_rule 决定 save_dir
         save_dir = self.dir_rule.deside_image_save_dir(
             photo.from_album,
             photo
         )
@@ -262,30 +259,22 @@
         PackerUtil.pack(self.deconstruct(), filepath)
 
     """
     下面是 build 方法
     """
 
     # 缓存
-    cache_jm_client = True
     jm_client_impl_mapping: Dict[str, Type[AbstractJmClient]] = {
         'html': JmHtmlClient,
         'api': JmApiClient,
     }
 
+    @field_cache("__jm_client_cache__")
     def build_jm_client(self, **kwargs) -> JmcomicClient:
-        if self.cache_jm_client is not True:
-            return self.new_jm_client(**kwargs)
-
-        client = self.jm_client_cache
-        if client is None:
-            client = self.new_jm_client(**kwargs)
-            self.jm_client_cache = client
-
-        return client
+        return self.new_jm_client(**kwargs)
 
     def new_jm_client(self, **kwargs) -> JmcomicClient:
         postman_conf: dict = self.client.postman.src_dict
 
         # support overwrite meta_data
         if len(kwargs) != 0:
             meta_data = postman_conf.get('meta_data', {})
```

### Comparing `jmcomic-2.1.5/src/jmcomic/jm_toolkit.py` & `jmcomic-2.1.6/src/jmcomic/jm_toolkit.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.5/src/jmcomic.egg-info/PKG-INFO` & `jmcomic-2.1.6/src/jmcomic.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.1.5
+Version: 2.1.6
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -39,43 +39,48 @@
 
   ```shell
   pip install -e ./
   ```
 
 ## 快速上手
 
-使用下面的两行代码，即可实现功能：把某个本子集（album）里的所有本子（photo）下载到本地
+使用下面的两行代码，即可实现功能：把某个本子（album）里的所有章节（photo）下载到本地
 
 ```python
 import jmcomic  # 导入此模块，需要先安装.
 jmcomic.download_album('422866')  # 传入要下载的album的id，即可下载整个album到本地.
 # 上面的这行代码，还有一个可选参数option: JmOption，表示配置项，
 # 配置项的作用是告诉程序下载时候的一些选择，
-# 比如，要下载到哪个文件夹，使用怎样的路径组织方式（比如[/作者/本子id/图片] 或者 [/作者/本子名称/图片]）.
+# 比如，要下载到哪个文件夹，使用怎样的路径组织规则（比如[/作者/本子id/图片] 或者 [/作者/本子名称/图片]）.
 # 如果没有配置，则会使用 JmOption.default()，下载的路径是[当前工作文件夹/本子名称/图片].
+# 如果你想要配置，请参考assets/config/和usgae/下的文档和示例.
 ```
 
 进一步的使用可以参考usage文件夹下的示例代码: `getting_started.py` `sample_usage.py`
 
 ## 项目特点
 
 - **绕过Cloudflare的反爬虫**
 - 支持使用**Github Action**下载漫画，不会编程都能用（[教程：使用Github Actions下载禁漫本子](./assets/docs/教程：使用Github%20Actions下载禁漫本子.md)）
 - 可配置性强
-
   - 不配置也能使用，十分方便
-  - 配置可以从**配置文件**生成，无需写Python代码
-  - 配置点有：`是否使用磁盘缓存`  `是否使用代理` `图片类型转换` `本子下载路径` `请求元信息（headers,cookies,重试次数）等 `
+  - 配置可以从**配置文件**生成，支持多种文件格式，无需写Python代码
+  - 配置点有：`是否使用磁盘缓存` `图片类型转换` `下载路径` `请求元信息（headers,cookies,代理）等 `
+- 可扩展性强
+  - 支持自定义本子/章节/图片下载前后的回调函数
+  - 支持自定义debug日志的开关/格式
+  - 支持自定义Option/Client/实体类
+- 支持重试和域名切换机制
 - 多线程下载（可细化到一图一线程，效率极高）
 - 跟进了JM最新的图片分割算法（2023-02-08）
 
 ## 使用小说明
 
 * Python >= 3.7
-* 项目只有代码注释，没有API文档。因此想深入高级地使用，自行看源码和改造代码叭 ^^_
+* 个人项目，文档和示例会有不及时之处，可以Issue提问
 
 ## 项目文件夹介绍
 
 * assets：存放一些非代码的资源文件
 
   * config：存放配置文件
   * docs：项目文档
```

