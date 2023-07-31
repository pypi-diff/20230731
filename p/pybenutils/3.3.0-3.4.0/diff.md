# Comparing `tmp/pybenutils-3.3.0.tar.gz` & `tmp/pybenutils-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybenutils-3.3.0.tar", last modified: Wed Jul 19 09:54:21 2023, max compression
+gzip compressed data, was "pybenutils-3.4.0.tar", last modified: Mon Jul 31 18:11:14 2023, max compression
```

## Comparing `pybenutils-3.3.0.tar` & `pybenutils-3.4.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 09:54:21.024885 pybenutils-3.3.0/
--rw-rw-rw-   0        0        0     1092 2023-07-06 12:04:25.000000 pybenutils-3.3.0/LICENSE
--rw-rw-rw-   0        0        0       27 2023-07-06 12:04:25.000000 pybenutils-3.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4311 2023-07-19 09:54:21.025882 pybenutils-3.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3465 2023-07-06 12:04:25.000000 pybenutils-3.3.0/README.md
--rw-rw-rw-   0        0        0       60 2023-07-06 12:04:25.000000 pybenutils-3.3.0/deploy_requirements.txt
--rw-rw-rw-   0        0        0      559 2023-07-06 12:04:25.000000 pybenutils-3.3.0/deployment_checklist.md
-drwxrwxrwx   0        0        0        0 2023-07-19 09:54:20.922160 pybenutils-3.3.0/pybenutils/
--rw-rw-rw-   0        0        0      153 2023-07-19 08:57:33.000000 pybenutils-3.3.0/pybenutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 09:54:20.952080 pybenutils-3.3.0/pybenutils/amazon_boto3/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/amazon_boto3/__init__.py
--rw-rw-rw-   0        0        0     7692 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/amazon_boto3/amazon_obj.py
-drwxrwxrwx   0        0        0        0 2023-07-19 09:54:20.960061 pybenutils-3.3.0/pybenutils/autogui/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/autogui/__init__.py
--rw-rw-rw-   0        0        0     1468 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/autogui/__main__.py
--rw-rw-rw-   0        0        0     6044 2023-07-19 08:57:24.000000 pybenutils-3.3.0/pybenutils/autogui/auto_gui_cls.py
-drwxrwxrwx   0        0        0        0 2023-07-19 09:54:20.979010 pybenutils-3.3.0/pybenutils/browsers/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/browsers/__init__.py
--rw-rw-rw-   0        0        0     1562 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/browsers/chrome.py
--rw-rw-rw-   0        0        0      939 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/browsers/firefox.py
--rw-rw-rw-   0        0        0    25553 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/browsers/selenium_utils.py
--rw-rw-rw-   0        0        0    19074 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/browsers/simple_browser_controller_cls.py
--rw-rw-rw-   0        0        0     2156 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/browsers/web_driver.py
--rw-rw-rw-   0        0        0     9474 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/browsers/windows_browsers_keywords.py
-drwxrwxrwx   0        0        0        0 2023-07-19 09:54:20.990976 pybenutils-3.3.0/pybenutils/network/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/network/__init__.py
--rw-rw-rw-   0        0        0     1926 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/network/download_manager.py
--rw-rw-rw-   0        0        0     3340 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/network/http_cert_info.py
--rw-rw-rw-   0        0        0    10654 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/network/s3_bucket_cls.py
--rw-rw-rw-   0        0        0     7073 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/network/ssh_helper.py
-drwxrwxrwx   0        0        0        0 2023-07-19 09:54:21.013914 pybenutils-3.3.0/pybenutils/os_operations/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/os_operations/__init__.py
--rw-rw-rw-   0        0        0     1279 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/os_operations/files_and_directories.py
--rw-rw-rw-   0        0        0    18804 2023-07-19 08:57:33.000000 pybenutils-3.3.0/pybenutils/os_operations/mac_application_control.py
--rw-rw-rw-   0        0        0     1467 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/os_operations/mac_input_control.py
--rw-rw-rw-   0        0        0     5506 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/os_operations/mac_operations.py
--rw-rw-rw-   0        0        0     3749 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/os_operations/mac_popup_handler.py
--rw-rw-rw-   0        0        0    11748 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/os_operations/process.py
--rw-rw-rw-   0        0        0    10361 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/os_operations/window_operations.py
--rw-rw-rw-   0        0        0     3103 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/useful.py
-drwxrwxrwx   0        0        0        0 2023-07-19 09:54:21.019899 pybenutils-3.3.0/pybenutils/utils_logger/
--rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/utils_logger/__init__.py
--rw-rw-rw-   0        0        0     1397 2023-07-06 12:04:25.000000 pybenutils-3.3.0/pybenutils/utils_logger/config_logger.py
-drwxrwxrwx   0        0        0        0 2023-07-19 09:54:20.946097 pybenutils-3.3.0/pybenutils.egg-info/
--rw-rw-rw-   0        0        0     4311 2023-07-19 09:54:20.000000 pybenutils-3.3.0/pybenutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1399 2023-07-19 09:54:20.000000 pybenutils-3.3.0/pybenutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 09:54:20.000000 pybenutils-3.3.0/pybenutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      213 2023-07-19 09:54:20.000000 pybenutils-3.3.0/pybenutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-19 09:54:20.000000 pybenutils-3.3.0/pybenutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      273 2023-07-06 12:04:25.000000 pybenutils-3.3.0/requirements.txt
--rw-rw-rw-   0        0        0      243 2023-07-19 09:54:21.027879 pybenutils-3.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2311 2023-07-19 08:57:33.000000 pybenutils-3.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-19 09:54:21.022891 pybenutils-3.3.0/tests/
--rw-rw-rw-   0        0        0      317 2023-07-06 12:04:25.000000 pybenutils-3.3.0/tests/test_self_import.py
+drwxrwxrwx   0        0        0        0 2023-07-31 18:11:14.544901 pybenutils-3.4.0/
+-rw-rw-rw-   0        0        0     1092 2023-07-06 12:04:25.000000 pybenutils-3.4.0/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-07-06 12:04:25.000000 pybenutils-3.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4311 2023-07-31 18:11:14.545899 pybenutils-3.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3465 2023-07-06 12:04:25.000000 pybenutils-3.4.0/README.md
+-rw-rw-rw-   0        0        0       60 2023-07-06 12:04:25.000000 pybenutils-3.4.0/deploy_requirements.txt
+-rw-rw-rw-   0        0        0      571 2023-07-31 08:16:17.000000 pybenutils-3.4.0/deployment_checklist.md
+drwxrwxrwx   0        0        0        0 2023-07-31 18:11:14.478083 pybenutils-3.4.0/pybenutils/
+-rw-rw-rw-   0        0        0      153 2023-07-31 18:10:53.000000 pybenutils-3.4.0/pybenutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 18:11:14.491045 pybenutils-3.4.0/pybenutils/amazon_boto3/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/amazon_boto3/__init__.py
+-rw-rw-rw-   0        0        0     7692 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/amazon_boto3/amazon_obj.py
+drwxrwxrwx   0        0        0        0 2023-07-31 18:11:14.496033 pybenutils-3.4.0/pybenutils/autogui/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/autogui/__init__.py
+-rw-rw-rw-   0        0        0     1468 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/autogui/__main__.py
+-rw-rw-rw-   0        0        0     6044 2023-07-19 08:57:24.000000 pybenutils-3.4.0/pybenutils/autogui/auto_gui_cls.py
+drwxrwxrwx   0        0        0        0 2023-07-31 18:11:14.510993 pybenutils-3.4.0/pybenutils/browsers/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/browsers/__init__.py
+-rw-rw-rw-   0        0        0     1762 2023-07-31 18:10:53.000000 pybenutils-3.4.0/pybenutils/browsers/chrome.py
+-rw-rw-rw-   0        0        0      939 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/browsers/firefox.py
+-rw-rw-rw-   0        0        0    25553 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/browsers/selenium_utils.py
+-rw-rw-rw-   0        0        0    19074 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/browsers/simple_browser_controller_cls.py
+-rw-rw-rw-   0        0        0     2156 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/browsers/web_driver.py
+-rw-rw-rw-   0        0        0     9474 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/browsers/windows_browsers_keywords.py
+drwxrwxrwx   0        0        0        0 2023-07-31 18:11:14.520967 pybenutils-3.4.0/pybenutils/network/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/network/__init__.py
+-rw-rw-rw-   0        0        0     1926 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/network/download_manager.py
+-rw-rw-rw-   0        0        0     3340 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/network/http_cert_info.py
+-rw-rw-rw-   0        0        0    10654 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/network/s3_bucket_cls.py
+-rw-rw-rw-   0        0        0     7073 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/network/ssh_helper.py
+drwxrwxrwx   0        0        0        0 2023-07-31 18:11:14.538918 pybenutils-3.4.0/pybenutils/os_operations/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/os_operations/__init__.py
+-rw-rw-rw-   0        0        0     1279 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/os_operations/files_and_directories.py
+-rw-rw-rw-   0        0        0    18804 2023-07-31 08:16:17.000000 pybenutils-3.4.0/pybenutils/os_operations/mac_application_control.py
+-rw-rw-rw-   0        0        0     1467 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/os_operations/mac_input_control.py
+-rw-rw-rw-   0        0        0     7497 2023-07-31 18:10:53.000000 pybenutils-3.4.0/pybenutils/os_operations/mac_operations.py
+-rw-rw-rw-   0        0        0     3749 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/os_operations/mac_popup_handler.py
+-rw-rw-rw-   0        0        0    11748 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/os_operations/process.py
+-rw-rw-rw-   0        0        0    10361 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/os_operations/window_operations.py
+-rw-rw-rw-   0        0        0     3103 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/useful.py
+drwxrwxrwx   0        0        0        0 2023-07-31 18:11:14.541910 pybenutils-3.4.0/pybenutils/utils_logger/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/utils_logger/__init__.py
+-rw-rw-rw-   0        0        0     1397 2023-07-06 12:04:25.000000 pybenutils-3.4.0/pybenutils/utils_logger/config_logger.py
+drwxrwxrwx   0        0        0        0 2023-07-31 18:11:14.487056 pybenutils-3.4.0/pybenutils.egg-info/
+-rw-rw-rw-   0        0        0     4311 2023-07-31 18:11:14.000000 pybenutils-3.4.0/pybenutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1399 2023-07-31 18:11:14.000000 pybenutils-3.4.0/pybenutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 18:11:14.000000 pybenutils-3.4.0/pybenutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      213 2023-07-31 18:11:14.000000 pybenutils-3.4.0/pybenutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-31 18:11:14.000000 pybenutils-3.4.0/pybenutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      273 2023-07-06 12:04:25.000000 pybenutils-3.4.0/requirements.txt
+-rw-rw-rw-   0        0        0      243 2023-07-31 18:11:14.546896 pybenutils-3.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2311 2023-07-31 08:16:17.000000 pybenutils-3.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 18:11:14.543904 pybenutils-3.4.0/tests/
+-rw-rw-rw-   0        0        0      317 2023-07-06 12:04:25.000000 pybenutils-3.4.0/tests/test_self_import.py
```

### Comparing `pybenutils-3.3.0/LICENSE` & `pybenutils-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybenutils-3.3.0/PKG-INFO` & `pybenutils-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybenutils
-Version: 3.3.0
+Version: 3.4.0
 Summary: PyBEN Utilities repository
 Home-page: https://github.com/DarkFlameBEN/pybenutils.git
 Author: Ben Moskovitch
 Author-email: "Ben Moskovitch" <darkflameben@gmail.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pybenutils-3.3.0/README.md` & `pybenutils-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pybenutils-3.3.0/deployment_checklist.md` & `pybenutils-3.4.0/deployment_checklist.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ### Deployment check list
 - Install deployment requirements
   - > python -m pip install -r deploy_requirements.txt -U
 - Test the package
   - > pytest .
   - > pytest . --pep8
 - Build the package
-  - > python setup.py sdist
+  - > python setup.py sdist bdist_wheel
 - README.md description test
  - > twine check dist/*
 - Deploy to repo (testpypi)
   - > python -m twine upload --repository testpypi dist/*
 - Test installation
   - > python -m pip install --index-url https://test.pypi.org/simple/ pybenutils -U
 - Deploy to repo (pypi)
```

### Comparing `pybenutils-3.3.0/pybenutils/amazon_boto3/amazon_obj.py` & `pybenutils-3.4.0/pybenutils/amazon_boto3/amazon_obj.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.3.0/pybenutils/autogui/__main__.py` & `pybenutils-3.4.0/pybenutils/autogui/__main__.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.3.0/pybenutils/autogui/auto_gui_cls.py` & `pybenutils-3.4.0/pybenutils/autogui/auto_gui_cls.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.3.0/pybenutils/browsers/chrome.py` & `pybenutils-3.4.0/pybenutils/browsers/chrome.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import subprocess
 import sys
+import time
 from subprocess import Popen
 from pybenutils.network.download_manager import download_url
+from pybenutils.os_operations.mac_operations import mount_image_mac, unmount_image_mac
 from pybenutils.utils_logger.config_logger import get_logger
 
 logger = get_logger()
 
 
 def update_chrome_browser():
     """Updating Chrome browser to its latest version. Returns True if successful, Raise exception on fail"""
@@ -19,13 +21,16 @@
 
         process = Popen(f'"{os.path.realpath("ChromeStandaloneSetup64.exe")}" /silent /install', shell=True)
         process.communicate()
         logger.info('Chrome installer finished')
     else:
         download_url('https://dl.google.com/dl/chrome/mac/universal/stable/gcea/googlechrome.dmg')
 
-        cmd = r'hdiutil attach googlechrome.dmg ' \
-              r'&& rm -R /Applications/Google Chrome.app ' \
-              r'&& cp -pPR "/Volumes/Google Chrome/Google Chrome.app" /Applications/'
+        mount_name = mount_image_mac('googlechrome.dmg')
+        time.sleep(5)
+        cmd = r'&& rm -R /Applications/Google Chrome.app ' \
+              fr'&& cp -pPR "/Volumes/{mount_name}/Google Chrome.app" /Applications/'
         p = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, stdin=subprocess.PIPE)
         p.communicate()
+        time.sleep(5)
+        unmount_image_mac(mount_name, retry=2)
     return True
```

### Comparing `pybenutils-3.3.0/pybenutils/browsers/firefox.py` & `pybenutils-3.4.0/pybenutils/browsers/firefox.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.3.0/pybenutils/browsers/selenium_utils.py` & `pybenutils-3.4.0/pybenutils/browsers/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.3.0/pybenutils/browsers/simple_browser_controller_cls.py` & `pybenutils-3.4.0/pybenutils/browsers/simple_browser_controller_cls.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.3.0/pybenutils/browsers/web_driver.py` & `pybenutils-3.4.0/pybenutils/browsers/web_driver.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.3.0/pybenutils/browsers/windows_browsers_keywords.py` & `pybenutils-3.4.0/pybenutils/browsers/windows_browsers_keywords.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.3.0/pybenutils/network/download_manager.py` & `pybenutils-3.4.0/pybenutils/network/download_manager.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.3.0/pybenutils/network/http_cert_info.py` & `pybenutils-3.4.0/pybenutils/network/http_cert_info.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.3.0/pybenutils/network/s3_bucket_cls.py` & `pybenutils-3.4.0/pybenutils/network/s3_bucket_cls.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.3.0/pybenutils/network/ssh_helper.py` & `pybenutils-3.4.0/pybenutils/network/ssh_helper.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.3.0/pybenutils/os_operations/files_and_directories.py` & `pybenutils-3.4.0/pybenutils/os_operations/files_and_directories.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.3.0/pybenutils/os_operations/mac_application_control.py` & `pybenutils-3.4.0/pybenutils/os_operations/mac_application_control.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.3.0/pybenutils/os_operations/mac_input_control.py` & `pybenutils-3.4.0/pybenutils/os_operations/mac_input_control.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.3.0/pybenutils/os_operations/mac_popup_handler.py` & `pybenutils-3.4.0/pybenutils/os_operations/mac_popup_handler.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.3.0/pybenutils/os_operations/process.py` & `pybenutils-3.4.0/pybenutils/os_operations/process.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.3.0/pybenutils/os_operations/window_operations.py` & `pybenutils-3.4.0/pybenutils/os_operations/window_operations.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.3.0/pybenutils/useful.py` & `pybenutils-3.4.0/pybenutils/useful.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.3.0/pybenutils/utils_logger/config_logger.py` & `pybenutils-3.4.0/pybenutils/utils_logger/config_logger.py`

 * *Files identical despite different names*

### Comparing `pybenutils-3.3.0/pybenutils.egg-info/PKG-INFO` & `pybenutils-3.4.0/pybenutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybenutils
-Version: 3.3.0
+Version: 3.4.0
 Summary: PyBEN Utilities repository
 Home-page: https://github.com/DarkFlameBEN/pybenutils.git
 Author: Ben Moskovitch
 Author-email: "Ben Moskovitch" <darkflameben@gmail.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pybenutils-3.3.0/pybenutils.egg-info/SOURCES.txt` & `pybenutils-3.4.0/pybenutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybenutils-3.3.0/setup.py` & `pybenutils-3.4.0/setup.py`

 * *Files identical despite different names*

