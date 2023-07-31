# Comparing `tmp/testApiGroup-1.0.0.0.tar.gz` & `tmp/testApiGroup-1.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testApiGroup-1.0.0.0.tar", last modified: Mon Jul 31 01:38:26 2023, max compression
+gzip compressed data, was "testApiGroup-1.0.0.1.tar", last modified: Mon Jul 31 05:23:17 2023, max compression
```

## Comparing `testApiGroup-1.0.0.0.tar` & `testApiGroup-1.0.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 01:38:26.788797 testApiGroup-1.0.0.0/
--rw-rw-rw-   0        0        0      129 2023-07-31 01:38:26.787930 testApiGroup-1.0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-31 01:38:26.788797 testApiGroup-1.0.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-31 01:38:26.701204 testApiGroup-1.0.0.0/testApiGroup/
--rw-rw-rw-   0        0        0      289 2023-07-31 01:38:25.000000 testApiGroup-1.0.0.0/testApiGroup/setup.py
--rw-rw-rw-   0        0        0     1112 2023-07-31 01:38:25.000000 testApiGroup-1.0.0.0/testApiGroup/testApiGroup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 01:38:26.784805 testApiGroup-1.0.0.0/testApiGroup.egg-info/
--rw-rw-rw-   0        0        0      129 2023-07-31 01:38:26.000000 testApiGroup-1.0.0.0/testApiGroup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-07-31 01:38:26.000000 testApiGroup-1.0.0.0/testApiGroup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 01:38:26.000000 testApiGroup-1.0.0.0/testApiGroup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-31 01:38:26.000000 testApiGroup-1.0.0.0/testApiGroup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-31 01:38:26.000000 testApiGroup-1.0.0.0/testApiGroup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 05:23:17.919393 testApiGroup-1.0.0.1/
+-rw-rw-rw-   0        0        0      129 2023-07-31 05:23:17.918570 testApiGroup-1.0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-31 05:23:17.919393 testApiGroup-1.0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 05:23:17.907393 testApiGroup-1.0.0.1/testApiGroup/
+-rw-rw-rw-   0        0        0      289 2023-07-31 05:23:17.000000 testApiGroup-1.0.0.1/testApiGroup/setup.py
+-rw-rw-rw-   0        0        0     1120 2023-07-31 05:23:17.000000 testApiGroup-1.0.0.1/testApiGroup/testApiGroup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:23:17.915392 testApiGroup-1.0.0.1/testApiGroup.egg-info/
+-rw-rw-rw-   0        0        0      129 2023-07-31 05:23:17.000000 testApiGroup-1.0.0.1/testApiGroup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-07-31 05:23:17.000000 testApiGroup-1.0.0.1/testApiGroup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 05:23:17.000000 testApiGroup-1.0.0.1/testApiGroup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-31 05:23:17.000000 testApiGroup-1.0.0.1/testApiGroup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-31 05:23:17.000000 testApiGroup-1.0.0.1/testApiGroup.egg-info/top_level.txt
```

### Comparing `testApiGroup-1.0.0.0/testApiGroup/testApiGroup.py` & `testApiGroup-1.0.0.1/testApiGroup/testApiGroup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,21 +10,21 @@
         self.url = http://localhost:8080
         logging.basicConfig(
             level=logging.DEBUG,  # 设置日志级别为DEBUG
             format='%(asctime)s - %(levelname)s - %(message)s',
             datefmt='%Y-%m-%d %H:%M:%S'
         )
 
-    def testApi(self, id):
+    def 用来测试的api(self, id):
        params = {'id':id}
        data = {"apiKey": "4fddfd63c67fa51ee7d5ff5e560b43d5", "currPage": 1, "pageSize": 10000}
        data["params"] = params
        self.httpSender(data)
 
-    def testApi2rd(self, id):
+    def fortest(self, id):
        params = {'id':id}
        data = {"apiKey": "5612de279f58b2a82502b35a6340596e", "currPage": 1, "pageSize": 10000}
        data["params"] = params
        self.httpSender(data)
```

