# Comparing `tmp/zerocap_api_new_test-0.1.4.tar.gz` & `tmp/zerocap_api_new_test-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zerocap_api_new_test-0.1.4.tar", last modified: Mon Jul 31 02:18:20 2023, max compression
+gzip compressed data, was "dist\zerocap_api_new_test-0.1.5.tar", last modified: Mon Jul 31 02:24:53 2023, max compression
```

## Comparing `zerocap_api_new_test-0.1.4.tar` & `zerocap_api_new_test-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 02:18:20.000000 zerocap_api_new_test-0.1.4/
--rw-rw-rw-   0        0        0    11523 2023-07-26 06:34:57.000000 zerocap_api_new_test-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0    18303 2023-07-31 02:18:20.000000 zerocap_api_new_test-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    15434 2023-07-31 02:13:00.000000 zerocap_api_new_test-0.1.4/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-31 02:18:20.000000 zerocap_api_new_test-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     2133 2023-07-31 02:18:13.000000 zerocap_api_new_test-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 02:18:20.000000 zerocap_api_new_test-0.1.4/zerocap_api_new_test/
--rw-rw-rw-   0        0        0      126 2023-07-29 09:52:06.000000 zerocap_api_new_test-0.1.4/zerocap_api_new_test/__init__.py
--rw-rw-rw-   0        0        0     8154 2023-07-29 09:52:06.000000 zerocap_api_new_test-0.1.4/zerocap_api_new_test/main.py
-drwxrwxrwx   0        0        0        0 2023-07-31 02:18:20.000000 zerocap_api_new_test-0.1.4/zerocap_api_new_test.egg-info/
--rw-rw-rw-   0        0        0    18303 2023-07-31 02:18:20.000000 zerocap_api_new_test-0.1.4/zerocap_api_new_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-31 02:18:20.000000 zerocap_api_new_test-0.1.4/zerocap_api_new_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 02:18:20.000000 zerocap_api_new_test-0.1.4/zerocap_api_new_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-31 02:18:20.000000 zerocap_api_new_test-0.1.4/zerocap_api_new_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-31 02:18:20.000000 zerocap_api_new_test-0.1.4/zerocap_api_new_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 02:24:53.000000 zerocap_api_new_test-0.1.5/
+-rw-rw-rw-   0        0        0    11523 2023-07-26 06:34:57.000000 zerocap_api_new_test-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0    18303 2023-07-31 02:24:53.000000 zerocap_api_new_test-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    15434 2023-07-31 02:13:00.000000 zerocap_api_new_test-0.1.5/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-31 02:24:53.000000 zerocap_api_new_test-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     2133 2023-07-31 02:24:49.000000 zerocap_api_new_test-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:24:53.000000 zerocap_api_new_test-0.1.5/zerocap_api_new_test/
+-rw-rw-rw-   0        0        0      126 2023-07-29 09:52:06.000000 zerocap_api_new_test-0.1.5/zerocap_api_new_test/__init__.py
+-rw-rw-rw-   0        0        0     8154 2023-07-29 09:52:06.000000 zerocap_api_new_test-0.1.5/zerocap_api_new_test/main.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:24:53.000000 zerocap_api_new_test-0.1.5/zerocap_api_new_test.egg-info/
+-rw-rw-rw-   0        0        0    18303 2023-07-31 02:24:53.000000 zerocap_api_new_test-0.1.5/zerocap_api_new_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-31 02:24:53.000000 zerocap_api_new_test-0.1.5/zerocap_api_new_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 02:24:53.000000 zerocap_api_new_test-0.1.5/zerocap_api_new_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-31 02:24:53.000000 zerocap_api_new_test-0.1.5/zerocap_api_new_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-31 02:24:53.000000 zerocap_api_new_test-0.1.5/zerocap_api_new_test.egg-info/top_level.txt
```

### Comparing `zerocap_api_new_test-0.1.4/LICENSE.txt` & `zerocap_api_new_test-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zerocap_api_new_test-0.1.4/PKG-INFO` & `zerocap_api_new_test-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerocap_api_new_test
-Version: 0.1.4
+Version: 0.1.5
 Summary: zerocap_api
 Home-page: https://zerocap.com/
 Author: zerocap
 Author-email: jiayu.gao@eigen.capital
 License: MIT
 Platform: all
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zerocap_api_new_test Version: 0.1.4 Summary:
+Metadata-Version: 2.1 Name: zerocap_api_new_test Version: 0.1.5 Summary:
 zerocap_api Home-page: https://zerocap.com/ Author: zerocap Author-email:
 jiayu.gao@eigen.capital License: MIT Platform: all Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE.txt # zerocap-
 api-new-test # Jump_restapi # Jump_websocket ``` æè¿°ä»ç» sdk install pip
 install zerocap-api-new-test ã ã ã ``` # restapi #### æ¥å£ææ¡£ ```
```

### Comparing `zerocap_api_new_test-0.1.4/README.rst` & `zerocap_api_new_test-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `zerocap_api_new_test-0.1.4/setup.py` & `zerocap_api_new_test-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         os.system('git tag v{0}'.format(about['__version__']))
         os.system('git push --tags')
 
         sys.exit()
 
 setup(
     name='zerocap_api_new_test',  # 包名
-    version='0.1.4',  # 版本号
+    version='0.1.5',  # 版本号
     description='zerocap_api',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='zerocap',
     author_email='jiayu.gao@eigen.capital',
     url='https://zerocap.com/',
     install_requires=REQUIRED,
```

### Comparing `zerocap_api_new_test-0.1.4/zerocap_api_new_test/main.py` & `zerocap_api_new_test-0.1.5/zerocap_api_new_test/main.py`

 * *Files identical despite different names*

### Comparing `zerocap_api_new_test-0.1.4/zerocap_api_new_test.egg-info/PKG-INFO` & `zerocap_api_new_test-0.1.5/zerocap_api_new_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerocap-api-new-test
-Version: 0.1.4
+Version: 0.1.5
 Summary: zerocap_api
 Home-page: https://zerocap.com/
 Author: zerocap
 Author-email: jiayu.gao@eigen.capital
 License: MIT
 Platform: all
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zerocap-api-new-test Version: 0.1.4 Summary:
+Metadata-Version: 2.1 Name: zerocap-api-new-test Version: 0.1.5 Summary:
 zerocap_api Home-page: https://zerocap.com/ Author: zerocap Author-email:
 jiayu.gao@eigen.capital License: MIT Platform: all Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE.txt # zerocap-
 api-new-test # Jump_restapi # Jump_websocket ``` æè¿°ä»ç» sdk install pip
 install zerocap-api-new-test ã ã ã ``` # restapi #### æ¥å£ææ¡£ ```
```

