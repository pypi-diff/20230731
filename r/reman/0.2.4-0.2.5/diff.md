# Comparing `tmp/reman-0.2.4.tar.gz` & `tmp/reman-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reman-0.2.4.tar", last modified: Wed Mar  1 14:14:48 2023, max compression
+gzip compressed data, was "reman-0.2.5.tar", last modified: Mon Jul 31 07:30:16 2023, max compression
```

## Comparing `reman-0.2.4.tar` & `reman-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ve        (1000) ve        (1000)        0 2023-03-01 14:14:48.091114 reman-0.2.4/
--rw-r--r--   0 ve        (1000) ve        (1000)      397 2023-03-01 14:14:48.091114 reman-0.2.4/PKG-INFO
--rw-r--r--   0 ve        (1000) ve        (1000)      112 2022-09-02 13:47:27.000000 reman-0.2.4/README.md
-drwxr-xr-x   0 ve        (1000) ve        (1000)        0 2023-03-01 14:14:48.091114 reman-0.2.4/bin/
--rw-r--r--   0 ve        (1000) ve        (1000)     5771 2023-03-01 14:13:53.000000 reman-0.2.4/bin/reman
-drwxr-xr-x   0 ve        (1000) ve        (1000)        0 2023-03-01 14:14:48.091114 reman-0.2.4/conanDefs/
--rw-r--r--   0 ve        (1000) ve        (1000)      893 2023-02-28 15:36:50.000000 reman-0.2.4/conanDefs/Variants.py
--rw-r--r--   0 ve        (1000) ve        (1000)        0 2023-02-28 15:36:50.000000 reman-0.2.4/conanDefs/__init__.py
-drwxr-xr-x   0 ve        (1000) ve        (1000)        0 2023-03-01 14:14:48.091114 reman-0.2.4/reman/
--rw-r--r--   0 ve        (1000) ve        (1000)     6413 2023-02-28 15:36:50.000000 reman-0.2.4/reman/ReMan.py
--rw-r--r--   0 ve        (1000) ve        (1000)        0 2022-09-02 13:47:27.000000 reman-0.2.4/reman/__init__.py
-drwxr-xr-x   0 ve        (1000) ve        (1000)        0 2023-03-01 14:14:48.091114 reman-0.2.4/reman.egg-info/
--rw-r--r--   0 ve        (1000) ve        (1000)      397 2023-03-01 14:14:48.000000 reman-0.2.4/reman.egg-info/PKG-INFO
--rw-r--r--   0 ve        (1000) ve        (1000)      249 2023-03-01 14:14:48.000000 reman-0.2.4/reman.egg-info/SOURCES.txt
--rw-r--r--   0 ve        (1000) ve        (1000)        1 2023-03-01 14:14:48.000000 reman-0.2.4/reman.egg-info/dependency_links.txt
--rw-r--r--   0 ve        (1000) ve        (1000)       25 2023-03-01 14:14:48.000000 reman-0.2.4/reman.egg-info/requires.txt
--rw-r--r--   0 ve        (1000) ve        (1000)       22 2023-03-01 14:14:48.000000 reman-0.2.4/reman.egg-info/top_level.txt
--rw-r--r--   0 ve        (1000) ve        (1000)       38 2023-03-01 14:14:48.091114 reman-0.2.4/setup.cfg
--rwxr-xr-x   0 ve        (1000) ve        (1000)     1016 2023-03-01 14:14:16.000000 reman-0.2.4/setup.py
+drwxr-xr-x   0 ve        (1000) ve        (1000)        0 2023-07-31 07:30:16.014364 reman-0.2.5/
+-rw-r--r--   0 ve        (1000) ve        (1000)      397 2023-07-31 07:30:16.014364 reman-0.2.5/PKG-INFO
+-rw-r--r--   0 ve        (1000) ve        (1000)      112 2022-09-02 13:47:27.000000 reman-0.2.5/README.md
+drwxr-xr-x   0 ve        (1000) ve        (1000)        0 2023-07-31 07:30:16.014364 reman-0.2.5/bin/
+-rw-r--r--   0 ve        (1000) ve        (1000)     5771 2023-03-01 16:19:10.000000 reman-0.2.5/bin/reman
+drwxr-xr-x   0 ve        (1000) ve        (1000)        0 2023-07-31 07:30:16.014364 reman-0.2.5/conanDefs/
+-rw-r--r--   0 ve        (1000) ve        (1000)      962 2023-07-31 07:28:36.000000 reman-0.2.5/conanDefs/Variants.py
+-rw-r--r--   0 ve        (1000) ve        (1000)        0 2023-02-28 15:36:50.000000 reman-0.2.5/conanDefs/__init__.py
+drwxr-xr-x   0 ve        (1000) ve        (1000)        0 2023-07-31 07:30:16.014364 reman-0.2.5/reman/
+-rw-r--r--   0 ve        (1000) ve        (1000)     6413 2023-02-28 15:36:50.000000 reman-0.2.5/reman/ReMan.py
+-rw-r--r--   0 ve        (1000) ve        (1000)        0 2022-09-02 13:47:27.000000 reman-0.2.5/reman/__init__.py
+drwxr-xr-x   0 ve        (1000) ve        (1000)        0 2023-07-31 07:30:16.014364 reman-0.2.5/reman.egg-info/
+-rw-r--r--   0 ve        (1000) ve        (1000)      397 2023-07-31 07:30:15.000000 reman-0.2.5/reman.egg-info/PKG-INFO
+-rw-r--r--   0 ve        (1000) ve        (1000)      249 2023-07-31 07:30:15.000000 reman-0.2.5/reman.egg-info/SOURCES.txt
+-rw-r--r--   0 ve        (1000) ve        (1000)        1 2023-07-31 07:30:15.000000 reman-0.2.5/reman.egg-info/dependency_links.txt
+-rw-r--r--   0 ve        (1000) ve        (1000)       25 2023-07-31 07:30:15.000000 reman-0.2.5/reman.egg-info/requires.txt
+-rw-r--r--   0 ve        (1000) ve        (1000)       22 2023-07-31 07:30:15.000000 reman-0.2.5/reman.egg-info/top_level.txt
+-rw-r--r--   0 ve        (1000) ve        (1000)       38 2023-07-31 07:30:16.014364 reman-0.2.5/setup.cfg
+-rwxr-xr-x   0 ve        (1000) ve        (1000)     1016 2023-07-31 07:29:34.000000 reman-0.2.5/setup.py
```

### Comparing `reman-0.2.4/bin/reman` & `reman-0.2.5/bin/reman`

 * *Files identical despite different names*

### Comparing `reman-0.2.4/conanDefs/Variants.py` & `reman-0.2.5/conanDefs/Variants.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 		pass
 
 	def createVariantsFile(self, target):
 		print("create variants.yml")
 		f = open("variants.yml", "w")
 		f.write("variants:\n")
 		match target: 
+			case "aurora":
+				f.write(f"  - \"-s board.product=aurora\"\n")
 			case "kp6tab":
 				f.write(f"  - \"-s board.product=kp6000\"\n")
 			case "taipan":
 				f.write(f"  - \"-s board.product=adept -s emv=True\"\n")
 				f.write(f"  - \"-s board.product=adept\"\n")
 				f.write(f"  - \"-s board.product=rugged -s emv=True\"\n")
 				f.write(f"  - \"-s board.product=rugged\"\n")
@@ -25,8 +27,8 @@
 				f.write(f"  - \"-s board.product=tp5800\"\n")
 				f.write(f"  - \"-s board.product=cp6500 -s emv=True\"\n")
 				f.write(f"  - \"-s board.product=cp6500\"\n")
 			case "cobra2":
 				f.write(f"  - \"-s board.product=cr6000\"\n")
 			case _:
 				f.write(f"  - \"\"\n")
-		f.close()
+		f.close()
```

### Comparing `reman-0.2.4/reman/ReMan.py` & `reman-0.2.5/reman/ReMan.py`

 * *Files identical despite different names*

### Comparing `reman-0.2.4/setup.py` & `reman-0.2.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="reman",
-    version="0.2.4",
+    version="0.2.5",
 
     description="ReMan build tools",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
```

