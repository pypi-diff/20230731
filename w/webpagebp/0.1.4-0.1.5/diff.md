# Comparing `tmp/webpagebp-0.1.4.tar.gz` & `tmp/webpagebp-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webpagebp-0.1.4.tar", max compression
+gzip compressed data, was "webpagebp-0.1.5.tar", max compression
```

## Comparing `webpagebp-0.1.4.tar` & `webpagebp-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1096 2022-10-14 16:09:17.578653 webpagebp-0.1.4/LICENSE
--rw-r--r--   0        0        0      423 2023-07-24 17:29:46.706405 webpagebp-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       12 2022-10-14 16:09:17.579153 webpagebp-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-01-03 20:49:12.324736 webpagebp-0.1.4/webpagebp/__init__.py
--rw-r--r--   0        0        0      929 2023-07-18 22:56:00.042430 webpagebp-0.1.4/webpagebp/browsers.py
--rw-r--r--   0        0        0        0 2022-12-30 22:04:46.955478 webpagebp-0.1.4/webpagebp/generic_browser/__init__.py
--rw-r--r--   0        0        0     2431 2023-07-19 15:14:40.063332 webpagebp-0.1.4/webpagebp/generic_browser/browser.py
--rw-r--r--   0        0        0     2090 2023-01-03 15:44:39.083890 webpagebp-0.1.4/webpagebp/generic_browser/old_browser.py
--rw-r--r--   0        0        0     2356 2023-07-19 15:15:49.321020 webpagebp-0.1.4/webpagebp/job.py
--rw-r--r--   0        0        0        0 2022-12-30 22:27:06.400627 webpagebp-0.1.4/webpagebp/scrapers/__init__.py
--rw-r--r--   0        0        0      945 2023-07-18 17:39:41.933029 webpagebp-0.1.4/webpagebp/scrapers/soup.py
--rw-r--r--   0        0        0        0 2022-12-30 21:41:00.943036 webpagebp-0.1.4/webpagebp/selenium_driver/__init__.py
--rw-r--r--   0        0        0     2364 2023-07-18 23:39:38.797351 webpagebp-0.1.4/webpagebp/selenium_driver/drivers.py
--rw-r--r--   0        0        0     1555 2023-07-18 22:56:00.041931 webpagebp-0.1.4/webpagebp/selenium_driver/generic_driver.py
--rw-r--r--   0        0        0      950 2023-07-19 14:50:18.873842 webpagebp-0.1.4/webpagebp/utils.py
--rw-r--r--   0        0        0     2640 2023-07-14 22:21:22.225050 webpagebp-0.1.4/webpagebp/webpage.py
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 webpagebp-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1096 2022-10-14 16:09:17.578653 webpagebp-0.1.5/LICENSE
+-rw-r--r--   0        0        0      423 2023-07-31 18:02:04.618784 webpagebp-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       12 2022-10-14 16:09:17.579153 webpagebp-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-01-03 20:49:12.324736 webpagebp-0.1.5/webpagebp/__init__.py
+-rw-r--r--   0        0        0      929 2023-07-18 22:56:00.042430 webpagebp-0.1.5/webpagebp/browsers.py
+-rw-r--r--   0        0        0        0 2022-12-30 22:04:46.955478 webpagebp-0.1.5/webpagebp/generic_browser/__init__.py
+-rw-r--r--   0        0        0     2431 2023-07-19 15:14:40.063332 webpagebp-0.1.5/webpagebp/generic_browser/browser.py
+-rw-r--r--   0        0        0     2090 2023-01-03 15:44:39.083890 webpagebp-0.1.5/webpagebp/generic_browser/old_browser.py
+-rw-r--r--   0        0        0     2757 2023-07-31 17:08:04.496777 webpagebp-0.1.5/webpagebp/job.py
+-rw-r--r--   0        0        0        0 2022-12-30 22:27:06.400627 webpagebp-0.1.5/webpagebp/scrapers/__init__.py
+-rw-r--r--   0        0        0      945 2023-07-18 17:39:41.933029 webpagebp-0.1.5/webpagebp/scrapers/soup.py
+-rw-r--r--   0        0        0        0 2022-12-30 21:41:00.943036 webpagebp-0.1.5/webpagebp/selenium_driver/__init__.py
+-rw-r--r--   0        0        0     2615 2023-07-31 17:30:56.096983 webpagebp-0.1.5/webpagebp/selenium_driver/drivers.py
+-rw-r--r--   0        0        0     1544 2023-07-31 17:11:34.580393 webpagebp-0.1.5/webpagebp/selenium_driver/generic_driver.py
+-rw-r--r--   0        0        0      950 2023-07-19 14:50:18.873842 webpagebp-0.1.5/webpagebp/utils.py
+-rw-r--r--   0        0        0     2640 2023-07-14 22:21:22.225050 webpagebp-0.1.5/webpagebp/webpage.py
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 webpagebp-0.1.5/PKG-INFO
```

### Comparing `webpagebp-0.1.4/LICENSE` & `webpagebp-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `webpagebp-0.1.4/webpagebp/browsers.py` & `webpagebp-0.1.5/webpagebp/browsers.py`

 * *Files identical despite different names*

### Comparing `webpagebp-0.1.4/webpagebp/generic_browser/browser.py` & `webpagebp-0.1.5/webpagebp/generic_browser/browser.py`

 * *Files identical despite different names*

### Comparing `webpagebp-0.1.4/webpagebp/generic_browser/old_browser.py` & `webpagebp-0.1.5/webpagebp/generic_browser/old_browser.py`

 * *Files identical despite different names*

### Comparing `webpagebp-0.1.4/webpagebp/job.py` & `webpagebp-0.1.5/webpagebp/job.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,14 +39,24 @@
 
 
 class Download(DefaultJob):
     def __init__(self, url: str, *args, **kwargs) -> None:
         super().__init__(url, browser=ChromeHBrowser, action='auto_download_and_exit', *args, **kwargs)
 
 
+class DownloadCh(DefaultJob):
+    def __init__(self, url: str, *args, **kwargs) -> None:
+        super().__init__(url, browser=ChromeHBrowser, action='auto_download_and_exit', *args, **kwargs)
+
+
+class DownloadFf(DefaultJob):
+    def __init__(self, url: str, *args, **kwargs) -> None:
+        super().__init__(url, browser=FirefoxHBrowser, action='auto_download_and_exit', *args, **kwargs)
+
+
 class Chrome(DefaultJob):
     def __init__(self, url: str, *args, **kwargs) -> None:
         super().__init__(url, browser=ChromeBrowser, *args, **kwargs)
 
 
 class ChromeH(DefaultJob):
     def __init__(self, url: str, *args, **kwargs) -> None:
```

### Comparing `webpagebp-0.1.4/webpagebp/scrapers/soup.py` & `webpagebp-0.1.5/webpagebp/scrapers/soup.py`

 * *Files identical despite different names*

### Comparing `webpagebp-0.1.4/webpagebp/selenium_driver/drivers.py` & `webpagebp-0.1.5/webpagebp/selenium_driver/drivers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 from selenium import webdriver
-from selenium.webdriver.chrome.service import Service
+from selenium.webdriver.chrome.service import Service as ChromeService
 from webdriver_manager.chrome import ChromeDriverManager
 from selenium.webdriver.chrome.options import Options as ChromeOptions
+from selenium.webdriver.firefox.service import Service as FirefoxService
 from webdriver_manager.firefox import GeckoDriverManager
 from selenium.webdriver.firefox.options import Options as FirefoxOptions
 
 from webpagebp.selenium_driver.generic_driver import _Driver
 
 
 class ChromeDriver(_Driver):
     def __init__(
         self, 
-        service: Service = Service(ChromeDriverManager().install()), 
+        service: ChromeService = ChromeService(ChromeDriverManager().install()), 
         webdriver: webdriver = webdriver.Chrome, 
         name = 'chrome', 
         *args, 
         **kwargs):
         super().__init__(service=service, webdriver=webdriver, name=name, *args, **kwargs)
 
     def load_startup_options(self) -> ChromeOptions:
         options = ChromeOptions()
         options.add_argument("log-level=3")
         options.add_argument("enable-automation")
         if self.run_headless:
             options.add_argument("--headless")
         options.add_argument("--window-size=1920,1080")
-        options.add_argument("--no-sandbox")
+        options.add_argument("--no-sandbox")              #bypass OS security model
         options.add_argument("--disable-extensions")
         options.add_argument("--dns-prefetch-disable")
         options.add_argument("--disable-gpu")
+        options.add_argument('--disable-dev-shm-usage')   #overcome limited resource problems
         options.add_argument("--silent")
         prefs = {"download.default_directory" : self.dir_path}
         options.add_experimental_option("prefs", prefs)
         return options
 
 
 class FirefoxDriver(_Driver):
     def __init__(
         self, 
-        service: Service = Service(GeckoDriverManager().install()),
+        service: FirefoxService = FirefoxService(GeckoDriverManager().install()),
         webdriver: webdriver = webdriver.Firefox,
         name = 'firefox', 
         *args, 
         **kwargs):
         super().__init__(service=service, webdriver=webdriver, name=name, *args, **kwargs)
 
     def load_startup_options(self) -> FirefoxOptions:
```

### Comparing `webpagebp-0.1.4/webpagebp/selenium_driver/generic_driver.py` & `webpagebp-0.1.5/webpagebp/selenium_driver/generic_driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from selenium.webdriver.common.by import By
-import os
 
 from webpagebp.utils import full_path
 
 
 class _Driver:
     def __init__(self, service=None, webdriver=None, name=None, dir='', headless=False, *args, **kwargs):
         self.dir_path = full_path(dir)
```

### Comparing `webpagebp-0.1.4/webpagebp/utils.py` & `webpagebp-0.1.5/webpagebp/utils.py`

 * *Files identical despite different names*

### Comparing `webpagebp-0.1.4/webpagebp/webpage.py` & `webpagebp-0.1.5/webpagebp/webpage.py`

 * *Files identical despite different names*

### Comparing `webpagebp-0.1.4/PKG-INFO` & `webpagebp-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: webpagebp
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Sergio Schmilovich
 Author-email: sergio.schmilovich@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: pytest (>=7.4.0,<8.0.0)
 Requires-Dist: selenium (>=4.10.0,<5.0.0)
-Requires-Dist: webdriver-manager (>=3.9.0,<4.0.0)
+Requires-Dist: webdriver-manager (>=4.0.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # webpage_bp
```

