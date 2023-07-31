# Comparing `tmp/kingunit_inspector-0.0.6.tar.gz` & `tmp/kingunit_inspector-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jiayu/Documents/Kingstar/KingUnit-Inspector/dist/.tmp-a7vs63k9/kingunit_inspector-0.0.6.tar", last modified: Fri Jul 28 06:31:44 2023, max compression
+gzip compressed data, was "/Users/jiayu/Documents/Kingstar/KingUnit-Inspector/dist/.tmp-9r6qrapg/kingunit_inspector-0.0.7.tar", last modified: Mon Jul 31 00:33:08 2023, max compression
```

## Comparing `kingunit_inspector-0.0.6.tar` & `kingunit_inspector-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 06:31:44.303296 kingunit_inspector-0.0.6/
--rw-r--r--   0 jiayu      (501) staff       (20)     9161 2023-07-19 06:48:32.000000 kingunit_inspector-0.0.6/LICENSE
--rw-r--r--   0 jiayu      (501) staff       (20)    10135 2023-07-28 06:31:44.303084 kingunit_inspector-0.0.6/PKG-INFO
--rw-r--r--   0 jiayu      (501) staff       (20)      111 2023-07-19 06:51:51.000000 kingunit_inspector-0.0.6/README.md
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 06:31:44.301563 kingunit_inspector-0.0.6/kingunit_inspector/
--rw-r--r--   0 jiayu      (501) staff       (20)        0 2023-07-19 07:08:08.000000 kingunit_inspector-0.0.6/kingunit_inspector/__init__.py
--rw-r--r--   0 jiayu      (501) staff       (20)     3478 2023-07-28 06:31:29.000000 kingunit_inspector-0.0.6/kingunit_inspector/inspector.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-28 06:31:44.302777 kingunit_inspector-0.0.6/kingunit_inspector.egg-info/
--rw-r--r--   0 jiayu      (501) staff       (20)    10135 2023-07-28 06:31:44.000000 kingunit_inspector-0.0.6/kingunit_inspector.egg-info/PKG-INFO
--rw-r--r--   0 jiayu      (501) staff       (20)      304 2023-07-28 06:31:44.000000 kingunit_inspector-0.0.6/kingunit_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 jiayu      (501) staff       (20)        1 2023-07-28 06:31:44.000000 kingunit_inspector-0.0.6/kingunit_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 jiayu      (501) staff       (20)        9 2023-07-28 06:31:44.000000 kingunit_inspector-0.0.6/kingunit_inspector.egg-info/requires.txt
--rw-r--r--   0 jiayu      (501) staff       (20)       19 2023-07-28 06:31:44.000000 kingunit_inspector-0.0.6/kingunit_inspector.egg-info/top_level.txt
--rw-r--r--   0 jiayu      (501) staff       (20)      443 2023-07-28 06:31:34.000000 kingunit_inspector-0.0.6/pyproject.toml
--rw-r--r--   0 jiayu      (501) staff       (20)       38 2023-07-28 06:31:44.303368 kingunit_inspector-0.0.6/setup.cfg
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-31 00:33:08.492366 kingunit_inspector-0.0.7/
+-rw-r--r--   0 jiayu      (501) staff       (20)     9161 2023-07-19 06:48:32.000000 kingunit_inspector-0.0.7/LICENSE
+-rw-r--r--   0 jiayu      (501) staff       (20)    10135 2023-07-31 00:33:08.492159 kingunit_inspector-0.0.7/PKG-INFO
+-rw-r--r--   0 jiayu      (501) staff       (20)      111 2023-07-19 06:51:51.000000 kingunit_inspector-0.0.7/README.md
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-31 00:33:08.490435 kingunit_inspector-0.0.7/kingunit_inspector/
+-rw-r--r--   0 jiayu      (501) staff       (20)        0 2023-07-19 07:08:08.000000 kingunit_inspector-0.0.7/kingunit_inspector/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     3468 2023-07-31 00:32:21.000000 kingunit_inspector-0.0.7/kingunit_inspector/inspector.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-31 00:33:08.491826 kingunit_inspector-0.0.7/kingunit_inspector.egg-info/
+-rw-r--r--   0 jiayu      (501) staff       (20)    10135 2023-07-31 00:33:08.000000 kingunit_inspector-0.0.7/kingunit_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 jiayu      (501) staff       (20)      304 2023-07-31 00:33:08.000000 kingunit_inspector-0.0.7/kingunit_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)        1 2023-07-31 00:33:08.000000 kingunit_inspector-0.0.7/kingunit_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)        9 2023-07-31 00:33:08.000000 kingunit_inspector-0.0.7/kingunit_inspector.egg-info/requires.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)       19 2023-07-31 00:33:08.000000 kingunit_inspector-0.0.7/kingunit_inspector.egg-info/top_level.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)      443 2023-07-31 00:32:33.000000 kingunit_inspector-0.0.7/pyproject.toml
+-rw-r--r--   0 jiayu      (501) staff       (20)       38 2023-07-31 00:33:08.492427 kingunit_inspector-0.0.7/setup.cfg
```

### Comparing `kingunit_inspector-0.0.6/LICENSE` & `kingunit_inspector-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kingunit_inspector-0.0.6/PKG-INFO` & `kingunit_inspector-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingunit_inspector
-Version: 0.0.6
+Version: 0.0.7
 Summary: KingUnit Inspector
 Author-email: 东南dnf <zjy2414@outlook.com>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `kingunit_inspector-0.0.6/kingunit_inspector/inspector.py` & `kingunit_inspector-0.0.7/kingunit_inspector/inspector.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,13 +101,13 @@
     if "expected" in test_case.keys() and test_case["expected"] != {}:
         for key in test_case["expected"].keys():
             assert (
                 key in response.json().keys()
             ), f"key: {key}, not found in response"
             assert (
                 str(response.json()[key]) == str(test_case["expected"][key])
-            ), f"response expected: {str(test_case['expected'][key])}, actual: {str(response.json()[key])}"
+            ), f"response expected: {str(test_case['expected'])}, actual: {str(response.json())}"
 
 
         # assert (
         #     response.json() == test_case["expected"]
         # ), f"response expected: {str(test_case['expected'])}, actual: {str(response.json())}"
```

### Comparing `kingunit_inspector-0.0.6/kingunit_inspector.egg-info/PKG-INFO` & `kingunit_inspector-0.0.7/kingunit_inspector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingunit-inspector
-Version: 0.0.6
+Version: 0.0.7
 Summary: KingUnit Inspector
 Author-email: 东南dnf <zjy2414@outlook.com>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

