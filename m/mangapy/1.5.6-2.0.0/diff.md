# Comparing `tmp/mangapy-1.5.6.tar.gz` & `tmp/mangapy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mangapy-1.5.6.tar", last modified: Sun Jan  9 11:46:25 2022, max compression
+gzip compressed data, was "mangapy-2.0.0.tar", last modified: Mon Jul 31 16:01:02 2023, max compression
```

## Comparing `mangapy-1.5.6.tar` & `mangapy-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2022-01-09 11:46:25.417925 mangapy-1.5.6/
--rw-r--r--   0 alessandro   (501) staff       (20)     1067 2019-12-11 18:08:50.000000 mangapy-1.5.6/LICENSE
--rw-r--r--   0 alessandro   (501) staff       (20)     3507 2022-01-09 11:46:25.417671 mangapy-1.5.6/PKG-INFO
--rw-r--r--   0 alessandro   (501) staff       (20)     2148 2020-05-19 10:13:10.000000 mangapy-1.5.6/README.md
-drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2022-01-09 11:46:25.415448 mangapy-1.5.6/mangapy/
--rw-r--r--   0 alessandro   (501) staff       (20)       51 2020-03-13 14:35:31.000000 mangapy-1.5.6/mangapy/__init__.py
--rw-r--r--   0 alessandro   (501) staff       (20)     4205 2022-01-09 11:39:55.000000 mangapy-1.5.6/mangapy/chapter_archiver.py
--rw-r--r--   0 alessandro   (501) staff       (20)     9498 2020-08-01 15:14:48.000000 mangapy-1.5.6/mangapy/cli.py
--rw-r--r--   0 alessandro   (501) staff       (20)     6674 2022-01-09 11:37:36.000000 mangapy-1.5.6/mangapy/fanfox.py
--rw-r--r--   0 alessandro   (501) staff       (20)     7408 2020-08-01 15:14:48.000000 mangapy-1.5.6/mangapy/mangapark.py
--rw-r--r--   0 alessandro   (501) staff       (20)      947 2019-12-29 17:33:25.000000 mangapy-1.5.6/mangapy/mangarepository.py
-drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2022-01-09 11:46:25.417261 mangapy-1.5.6/mangapy.egg-info/
--rw-r--r--   0 alessandro   (501) staff       (20)     3507 2022-01-09 11:46:25.000000 mangapy-1.5.6/mangapy.egg-info/PKG-INFO
--rw-r--r--   0 alessandro   (501) staff       (20)      358 2022-01-09 11:46:25.000000 mangapy-1.5.6/mangapy.egg-info/SOURCES.txt
--rw-r--r--   0 alessandro   (501) staff       (20)        1 2022-01-09 11:46:25.000000 mangapy-1.5.6/mangapy.egg-info/dependency_links.txt
--rw-r--r--   0 alessandro   (501) staff       (20)       58 2022-01-09 11:46:25.000000 mangapy-1.5.6/mangapy.egg-info/entry_points.txt
--rw-r--r--   0 alessandro   (501) staff       (20)       32 2022-01-09 11:46:25.000000 mangapy-1.5.6/mangapy.egg-info/requires.txt
--rw-r--r--   0 alessandro   (501) staff       (20)        8 2022-01-09 11:46:25.000000 mangapy-1.5.6/mangapy.egg-info/top_level.txt
--rw-r--r--   0 alessandro   (501) staff       (20)      100 2021-03-23 11:11:45.000000 mangapy-1.5.6/pyproject.toml
--rw-r--r--   0 alessandro   (501) staff       (20)       38 2022-01-09 11:46:25.418020 mangapy-1.5.6/setup.cfg
--rw-r--r--   0 alessandro   (501) staff       (20)     1107 2022-01-09 11:44:12.000000 mangapy-1.5.6/setup.py
+drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2023-07-31 16:01:02.354396 mangapy-2.0.0/
+-rw-r--r--   0 alessandro   (501) staff       (20)     1067 2019-12-11 18:08:50.000000 mangapy-2.0.0/LICENSE
+-rw-r--r--   0 alessandro   (501) staff       (20)     2603 2023-07-31 16:01:02.354077 mangapy-2.0.0/PKG-INFO
+-rw-r--r--   0 alessandro   (501) staff       (20)     1946 2023-07-31 15:59:06.000000 mangapy-2.0.0/README.md
+drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2023-07-31 16:01:02.350561 mangapy-2.0.0/mangapy/
+-rw-r--r--   0 alessandro   (501) staff       (20)       51 2020-03-13 14:35:31.000000 mangapy-2.0.0/mangapy/__init__.py
+-rw-r--r--   0 alessandro   (501) staff       (20)     4524 2023-07-31 15:59:06.000000 mangapy-2.0.0/mangapy/chapter_archiver.py
+-rw-r--r--   0 alessandro   (501) staff       (20)     9061 2023-07-31 15:59:06.000000 mangapy-2.0.0/mangapy/cli.py
+-rw-r--r--   0 alessandro   (501) staff       (20)     6714 2023-07-31 15:59:06.000000 mangapy-2.0.0/mangapy/fanfox.py
+-rw-r--r--   0 alessandro   (501) staff       (20)      994 2023-07-31 15:59:06.000000 mangapy-2.0.0/mangapy/mangarepository.py
+drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2023-07-31 16:01:02.353131 mangapy-2.0.0/mangapy.egg-info/
+-rw-r--r--   0 alessandro   (501) staff       (20)     2603 2023-07-31 16:01:02.000000 mangapy-2.0.0/mangapy.egg-info/PKG-INFO
+-rw-r--r--   0 alessandro   (501) staff       (20)      358 2023-07-31 16:01:02.000000 mangapy-2.0.0/mangapy.egg-info/SOURCES.txt
+-rw-r--r--   0 alessandro   (501) staff       (20)        1 2023-07-31 16:01:02.000000 mangapy-2.0.0/mangapy.egg-info/dependency_links.txt
+-rw-r--r--   0 alessandro   (501) staff       (20)       45 2023-07-31 16:01:02.000000 mangapy-2.0.0/mangapy.egg-info/entry_points.txt
+-rw-r--r--   0 alessandro   (501) staff       (20)       32 2023-07-31 16:01:02.000000 mangapy-2.0.0/mangapy.egg-info/requires.txt
+-rw-r--r--   0 alessandro   (501) staff       (20)        8 2023-07-31 16:01:02.000000 mangapy-2.0.0/mangapy.egg-info/top_level.txt
+-rw-r--r--   0 alessandro   (501) staff       (20)      100 2021-03-23 11:11:45.000000 mangapy-2.0.0/pyproject.toml
+-rw-r--r--   0 alessandro   (501) staff       (20)       38 2023-07-31 16:01:02.354493 mangapy-2.0.0/setup.cfg
+-rw-r--r--   0 alessandro   (501) staff       (20)     1109 2023-07-31 15:59:06.000000 mangapy-2.0.0/setup.py
+drwxr-xr-x   0 alessandro   (501) staff       (20)        0 2023-07-31 16:01:02.353553 mangapy-2.0.0/tests/
+-rw-r--r--   0 alessandro   (501) staff       (20)     2282 2020-07-31 15:33:31.000000 mangapy-2.0.0/tests/test_fanfox.py
```

### Comparing `mangapy-1.5.6/LICENSE` & `mangapy-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mangapy-1.5.6/README.md` & `mangapy-2.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # mangapy
 
 Manga downloader supporting the following sources:
 
 - fanfox.net
-- mangapark.net
 
 ## Installation
 
 ```
 pip install --upgrade mangapy
 ```
 
@@ -32,32 +31,32 @@
 
 Downloads Bleach chatper 1 as images inside the *Downloads* folder (from Fanfox source).  
 
 ```
 mangapy title bleach -c 1 -o ~/Downloads
 ```
 
-Downloads Bleach chatpers from 0 to 10 (included) as images inside the *Downloads* folder using MangaPark as source.  
+Downloads Bleach chatpers from 0 to 10 (included) as images inside the *Downloads* folder using Fanfox as source.  
 
 ```
-mangapy title bleach -c 0-10 -o ~/Downloads -s mangapark
+mangapy title bleach -c 0-10 -o ~/Downloads -s fanfox
 ```
 
 You may need a proxy to download certain manga, to do so use the option *-p or --proxy*:
 Downloads the last One Piece chapter as images inside the *Downloads* folder (from Fanfox source) using the proxy during the search.  
 
 ```
 mangapy title "one piece" -o ~/Downloads -p '{"http": "194.226.34.132:8888", "https": "194.226.34.132:8888"}'
 ```
 
 ### YAML
 
 Mangapy let you download multiple manga chapters as images (default) or pdfs from a *.yaml* file.
 For every manga you can choose:
-- source (*fanfox* or *mangapark*)
+- source (*fanfox*)
 - whether or not save the manga as a single pdf
 - which chapter to download (single, range, all, last)
 
 ```
 mangapy yaml PATH_TO_YOUR_YAML_FILE
 ```
 
@@ -74,15 +73,8 @@
     download_single_chapter: "10"
   - title: "naruto"
     pdf: true
     download_chapters: "10-13"
   - title: "black clover"
     download_all_chapters: True
     pdf: true
- mangapark:
-  - title: "black clover tabata yuuki"
-    pdf: true
-    download_last_chapter: True
-  - title: "Daiya no A"
-    pdf: true
-    download_chapters: "111-"
 ```
```

### Comparing `mangapy-1.5.6/mangapy/chapter_archiver.py` & `mangapy-2.0.0/mangapy/chapter_archiver.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import logging
 import os
 import re
 import requests
 import shutil
+from collections.abc import Mapping
 from functools import partial
 from tqdm import tqdm
 from PIL import Image
 from urllib.parse import urlparse
 from mangapy.mangarepository import Chapter, Page
 from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
@@ -14,31 +16,31 @@
 class ChapterArchiver(object):
     session = requests.Session()
 
     def __init__(self, path: str, max_workers=1):
         self.max_workers = max_workers
         self.path = Path(path).expanduser()
 
-    def archive(self, chapter: Chapter, pdf: bool):
+    def archive(self, chapter: Chapter, pdf: bool, headers: Mapping[str, str | bytes | None] | None):
         if pdf:
             images_path = self.path.joinpath('.images')
         else:
             images_path = self.path.joinpath('images')
 
-        isChapterNumberInt = isinstance(chapter.number, int) or chapter.number.is_integer()
-        chapter_name = str(int(chapter.number)) if isChapterNumberInt else str(chapter.number)
+        isChapterNumberAnInt = isinstance(chapter.number, int) or chapter.number.is_integer()
+        chapter_name = str(int(chapter.number)) if isChapterNumberAnInt else str(chapter.number)
         chapter_images_path = images_path.joinpath(str(chapter.number))
         chapter_images_path.mkdir(parents=True, exist_ok=True)
         pages = chapter.pages()
         if pages is None or not len(pages):
             print("🆘  {0} doesn't have any pages and it will be skipped.".format(chapter_name))
             return
 
         description = ('Chapter {0}'.format(chapter_name))
-        func = partial(self._save_image, chapter_images_path)  # currying
+        func = partial(self._save_image, chapter_images_path, headers)  # currying
 
         if pdf:
             pdf_path = self.path.joinpath('pdf')
             chapter_pdf_file_path = pdf_path.joinpath(chapter_name + '.pdf')
             if os.path.isfile(chapter_pdf_file_path):
                 print("⏺  {0} already downloaded and it will skipped.".format(chapter_name))
                 return  # early exit if the file is already on disk
@@ -49,34 +51,35 @@
         if pdf:
             pdf_path = self.path.joinpath('pdf')
             pdf_path.mkdir(parents=True, exist_ok=True)
             chapter_pdf_file_path = pdf_path.joinpath(chapter_name + '.pdf')
             self._create_chapter_pdf(chapter_images_path, chapter_pdf_file_path)
             shutil.rmtree(chapter_images_path, ignore_errors=True)
 
-    def _fetch_image(self, url: str):
-        response = self.session.get(url, verify=False)
+    def _fetch_image(self, url: str, headers: Mapping[str, str | bytes | None] | None):
+        response = self.session.get(url, verify=False, headers=headers)
         if response.status_code != 200:
             return None
         return response.content
 
-    def _save_image(self, image_path: Path, page: Page):
+    def _save_image(self, image_path: Path, headers: Mapping[str, str | bytes | None] | None, page: Page):
         file_name = str(page.number)
         image_url = page.url
         file_ext = urlparse(image_url).path.split('.')[-1]
         file_path = image_path.joinpath(file_name + '.' + file_ext)
         if os.path.isfile(file_path):
             return  # early exit if the file is already on disk
 
         if image_url.startswith('//'):
             image_url = 'http:' + image_url
 
-        data = self._fetch_image(image_url)
+        data = self._fetch_image(image_url, headers=headers)
 
         if data is None:
+            logging.error("Can't download page {0}".format(file_name))
             return
 
         output = open(file_path, "wb")
         output.write(data)
         output.close()
 
     def _create_chapter_pdf(self, chapter_images_path: Path, pdf_path: Path):
```

### Comparing `mangapy-1.5.6/mangapy/cli.py` & `mangapy-2.0.0/mangapy/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import argparse
 import yaml
 import json
 import logging
 import os
 import pkg_resources
 import sys
-from mangapy.mangapark import MangaParkRepository
 from mangapy.fanfox import FanFoxRepository
 from mangapy.chapter_archiver import ChapterArchiver
 from mangapy import log
 from pathlib import Path
-
+from typing import Tuple
 
 version = pkg_resources.require("mangapy")[0].version
 default_path_to_download_folder = str(os.path.join(Path.home(), "Downloads", "mangapy"))
 
 
 def cmd_parse():
     """Returns parsed arguments from command line"""
@@ -33,15 +32,15 @@
     args_parser.add_argument('-d', '--debug', action='store_true', help="set log to DEBUG level")
     args_parser.add_argument('--pdf', action='store_true', help="create a pdf for each chapter")
 
     args_parser.add_argument('-p', '--proxy', type=json.loads, help="use a proxy to download the chapters")
     group = args_parser.add_mutually_exclusive_group()
     group.add_argument('-a', '--all', action='store_true', help="download all chapters available")
     group.add_argument('-c', '--chapter', type=str, help="chapter(s) number to download")
-    
+
     parser.add_argument('-v', '--version',
                         action='version',
                         version='{0} {1}'.format(parser.prog, version),
                         help="show program version and exit")
 
     args = parser.parse_args()
     return args
@@ -75,15 +74,15 @@
         return False
 
     def download_all(self) -> bool:
         if 'download_all_chapters' in self.__dict__.keys():
             return self.__dict__['download_all_chapters']
         return False
 
-    def download_range(self) -> (float, float):
+    def download_range(self) -> Tuple[float, float]:
         if 'download_chapters' in self.__dict__.keys():
             chapters = self.__dict__['download_chapters']
             chapters = chapters.split('-')
             begin = None
             end = None
             if len(chapters) == 2:
                 begin = float(chapters[0])
@@ -118,23 +117,15 @@
             if 'fanfox' in dictionary.keys():
                 for download in list(map(lambda manga: MangaDownload(**manga), dictionary['fanfox'])):
                     download.source = 'fanfox'
                     download.enable_debug_log = debug_log
                     download.output = output
                     download.proxy = proxy
                     start_download(download)
-            
-            if 'mangapark' in dictionary.keys():
-                for download in list(map(lambda manga: MangaDownload(**manga), dictionary['mangapark'])):
-                    download.source = 'mangapark'
-                    download.enable_debug_log = debug_log
-                    download.output = output
-                    download.proxy = proxy
-                    start_download(download)
-    except Exception as error:   
+    except Exception as error:
         print(error)
 
 
 def main_title(args: argparse.Namespace):
     download = MangaDownload()
     download.title = args.manga_title.strip()
     download.output = args.out.strip()
@@ -154,15 +145,15 @@
     download.proxy = None
     if args.proxy:
         if 'http' and 'https' in args.proxy.keys():
             print('Setting proxy')
             download.proxy = args.proxy
         else:
             print('The proxy is not in the right format and it will not be used.')
-            
+
     if args.all:
         download.download_all_chapters = True
 
     elif args.chapter:
         chapters = args.chapter.split('-')
         if len(chapters) == 2:
             download.download_chapters = args.chapter
@@ -176,30 +167,30 @@
 
 def start_download(download: MangaDownload):
     if download.enable_debug_log:
         log.setLevel(logging.DEBUG)
     else:
         log.setLevel(logging.ERROR)
 
+    headers = None
+
     if download.source is None:
         repository = FanFoxRepository()
         repository_directory = 'fanfox'
+        headers = {"Referer": "http://fanfox.net/"}
         max_workers = 1  # to avoid bot detection
     else:
         source = download.source.strip().lower()
         if source == 'fanfox':
             repository = FanFoxRepository()
             repository_directory = source
             max_workers = 1  # to avoid bot detection
-        elif source == 'mangapark':
-            repository = MangaParkRepository()
-            repository_directory = source
-            max_workers = 5
+            headers = {"Referer": "{0}".format(repository.base_url)}
         else:
-            sys.exit('source is missing')
+            sys.exit('Source {0} is missing'.format(source))
 
     if download.proxy:
         repository.proxies = download.proxy
 
     print('🔎  Searching for {0} in {1}...'.format(download.title, download.source))
     try:
         manga = repository.search(download.title)
@@ -237,24 +228,24 @@
         for index, chapter in enumerate(manga.chapters):
             if chapter.number == range_begin:
                 start = index
             if range_end and chapter.number == range_end:
                 stop = index + 1
         for chapter in manga.chapters[start:stop]:
             chapters.append(chapter)
- 
+
     else:  # manga._download_last()
         last_chapter = manga.last_chapter
         chapters.append(last_chapter)
 
     print('⬇️  Download started.')
     archiver = ChapterArchiver(directory, max_workers=max_workers)
     for chapter in chapters:
         try:
-            archiver.archive(chapter, download.save_as_pdf())
+            archiver.archive(chapter, download.save_as_pdf(), headers)
         except Exception as e:
             logging.error(str(e))
 
     print('🎉  Download finished.')
 
 
 if __name__ == '__main__':
@@ -263,13 +254,13 @@
     sys.argv.insert(1, 'yaml')
     sys.argv.insert(2, yaml_file)
 
     # sys.argv.insert(1, 'title')
     # sys.argv.insert(2, 'jujutsu kaisen')
     # sys.argv.insert(3, '-o ~/Downloads/mangapy_test')
     # sys.argv.insert(4, '-c 1-100')
-    # sys.argv.insert(5, '-s mangapark')
+    # sys.argv.insert(5, '-s fanfox')
     # sys.argv.insert(6, '--pdf')
     # sys.argv.insert(7, '--debug')
     # sys.argv.insert(8, '-p {"http": "http://31.14.131.70:8080", "https": "http://31.14.131.70:8080"}')
 
     main()
```

### Comparing `mangapy-1.5.6/mangapy/fanfox.py` & `mangapy-2.0.0/mangapy/fanfox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 import requests
 from mangapy import log
 from mangapy.mangarepository import MangaRepository, Manga, Chapter, Page
 from bs4 import BeautifulSoup
+from typing import List
 
 
 def unpack(p, a, c, k, e=None, d=None):
     def baseN(num, b, numerals="0123456789abcdefghijklmnopqrstuvwxyz"):
         return ((num == 0) and numerals[0]) or (baseN(num // b, b, numerals).lstrip(numerals[0]) + numerals[num % b])
 
     while (c):
@@ -30,15 +31,15 @@
         self._session = requests.Session()
         headers = {
             'Accept': 'text/html,application/xhtml+xml,application/xml;q=1.0,image/webp,image/apng,*/*;q=1.0',
             'Accept-Encoding': 'gzip, deflate',
             'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) '
                           'Chrome/60.0.3112.101 Safari/537.36',
             'Accept-Language': 'ru-RU,ru;q=0.8,en-US;q=0.5,en;q=0.3',
-            'Referer': 'http://fanfox.net',
+            'Referer': '{0}'.format(self.base_url),
             'Connection': 'keep-alive'
         }
 
         self._session.cookies['isAdult'] = '1'
         self._session.headers = headers
         self._session.proxies = self.proxies
         return self._session
@@ -58,15 +59,15 @@
             absolute_url = "{0}{1}".format(self.base_url, url)
             number = float(number)
             chapter = FanFoxChapter(absolute_url, number, self.session)
             manga_chapters.append(chapter)
 
         return manga_chapters
 
-    def search(self, manga_name) -> [Manga]:
+    def search(self, manga_name) -> List[Manga]:
         # support alphanumeric names with multiple words
         manga_name_adjusted = re.sub(r'[^A-Za-z0-9]+', '_', re.sub(r'^[^A-Za-z0-9]+|[^A-Za-z0-9]+$', '', manga_name)).lower()
         manga_url = "{0}/manga/{1}".format(self.base_url, manga_name_adjusted)
         response = self.session.get(url=manga_url)
 
         if response is None or response.status_code != 200:
             return None
@@ -146,15 +147,15 @@
         return content
 
     def _parse_links(self, data):
         base_path = re.search(r'pix="(.+?)"', data).group(1)
         images = re.findall(r'"(/\w.+?)"', data)
         return [base_path + i for i in images]
 
-    def pages(self) -> [Page]:
+    def pages(self) -> List[Page]:
         base_url = self.first_page_url[:self.first_page_url.rfind('/')]
         response = self.session.get(self.first_page_url)
 
         if response is None or response.status_code != 200:
             return None
 
         content = response.text
```

### Comparing `mangapy-1.5.6/setup.py` & `mangapy-2.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 
 setup(
     author="Alessandro Marzoli",
     author_email="me@alessandromarzoli.com",
     name='mangapy',
     license="MIT",
     description='Manga downloader',
-    version='1.5.6',
+    version='2.0.0',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/alemar11/mangapy',
     packages=find_packages(),
-    python_requires=">=3.7",
+    python_requires=">=3.11",
     install_requires=['bs4', 'pillow', 'pyyaml', 'requests', 'tqdm'],
     classifiers=[
         # (https://pypi.python.org/pypi?%3Aaction=list_classifiers)
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Games/Entertainment',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Intended Audience :: End Users/Desktop',
     ],
     entry_points="""
     [console_scripts]
     mangapy = mangapy.cli:main
```

