# Comparing `tmp/hapm-0.0.4.tar.gz` & `tmp/hapm-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hapm-0.0.4.tar", last modified: Fri Feb 17 23:50:40 2023, max compression
+gzip compressed data, was "hapm-0.0.5.tar", last modified: Mon Jul 31 08:59:17 2023, max compression
```

## Comparing `hapm-0.0.4.tar` & `hapm-0.0.5.tar`

### file list

```diff
@@ -1,36 +1,48 @@
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-02-17 23:50:40.128508 hapm-0.0.4/
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1529 2023-02-17 23:50:40.128368 hapm-0.0.4/PKG-INFO
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1169 2023-02-17 22:09:27.000000 hapm-0.0.4/README.md
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-02-17 23:50:40.128006 hapm-0.0.4/hapm.egg-info/
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1529 2023-02-17 23:50:40.000000 hapm-0.0.4/hapm.egg-info/PKG-INFO
--rw-r--r--   0 mishamyrt   (501) staff       (20)      735 2023-02-17 23:50:40.000000 hapm-0.0.4/hapm.egg-info/SOURCES.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)        1 2023-02-17 23:50:40.000000 hapm-0.0.4/hapm.egg-info/dependency_links.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)       53 2023-02-17 23:50:40.000000 hapm-0.0.4/hapm.egg-info/requires.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)        8 2023-02-17 23:50:40.000000 hapm-0.0.4/hapm.egg-info/top_level.txt
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-02-17 23:50:40.124797 hapm-0.0.4/libhapm/
--rw-r--r--   0 mishamyrt   (501) staff       (20)        0 2023-02-17 18:11:43.000000 hapm-0.0.4/libhapm/__init__.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-02-17 23:50:40.125332 hapm-0.0.4/libhapm/integrations/
--rw-r--r--   0 mishamyrt   (501) staff       (20)       71 2023-02-17 18:15:35.000000 hapm-0.0.4/libhapm/integrations/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     2855 2023-02-17 22:50:09.000000 hapm-0.0.4/libhapm/integrations/integration.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     2636 2023-02-17 21:43:32.000000 hapm-0.0.4/libhapm/integrations/module.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-02-17 23:50:40.126143 hapm-0.0.4/libhapm/packages/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      194 2023-02-17 20:38:25.000000 hapm-0.0.4/libhapm/packages/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     2158 2023-02-17 23:47:20.000000 hapm-0.0.4/libhapm/packages/controller.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      621 2023-02-17 20:47:38.000000 hapm-0.0.4/libhapm/packages/lock.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-02-17 23:50:40.126698 hapm-0.0.4/libhapm/packages/manifest/
--rw-r--r--   0 mishamyrt   (501) staff       (20)       30 2023-02-17 19:38:47.000000 hapm-0.0.4/libhapm/packages/manifest/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      605 2023-02-17 21:37:27.000000 hapm-0.0.4/libhapm/packages/manifest/manifest.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1156 2023-02-17 20:47:13.000000 hapm-0.0.4/libhapm/packages/manifest/parse.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      231 2023-02-17 19:34:22.000000 hapm-0.0.4/libhapm/packages/manifest/types.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      994 2023-02-17 21:38:57.000000 hapm-0.0.4/libhapm/packages/module.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      157 2023-02-17 17:58:30.000000 hapm-0.0.4/libhapm/packages/package.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      182 2023-02-12 10:41:34.000000 hapm-0.0.4/libhapm/packages/path.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1906 2023-02-12 11:01:40.000000 hapm-0.0.4/libhapm/progress.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-02-17 23:50:40.127231 hapm-0.0.4/libhapm/repository/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      151 2023-02-12 13:11:52.000000 hapm-0.0.4/libhapm/repository/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1400 2023-02-12 13:49:44.000000 hapm-0.0.4/libhapm/repository/sync.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      931 2023-02-11 18:00:13.000000 hapm-0.0.4/libhapm/versions.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-02-17 23:50:40.128153 hapm-0.0.4/scripts/
--rwxr-xr-x   0 mishamyrt   (501) staff       (20)     1597 2023-02-17 23:48:58.000000 hapm-0.0.4/scripts/hapm
--rw-r--r--   0 mishamyrt   (501) staff       (20)       38 2023-02-17 23:50:40.128557 hapm-0.0.4/setup.cfg
--rw-r--r--   0 mishamyrt   (501) staff       (20)      953 2023-02-17 22:43:54.000000 hapm-0.0.4/setup.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-31 08:59:17.349519 hapm-0.0.5/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1394 2023-07-31 08:59:17.349363 hapm-0.0.5/PKG-INFO
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1034 2023-02-20 21:55:23.000000 hapm-0.0.5/README.md
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-31 08:59:17.348722 hapm-0.0.5/hapm.egg-info/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1394 2023-07-31 08:59:17.000000 hapm-0.0.5/hapm.egg-info/PKG-INFO
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      918 2023-07-31 08:59:17.000000 hapm-0.0.5/hapm.egg-info/SOURCES.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)        1 2023-07-31 08:59:17.000000 hapm-0.0.5/hapm.egg-info/dependency_links.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       79 2023-07-31 08:59:17.000000 hapm-0.0.5/hapm.egg-info/requires.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)        8 2023-07-31 08:59:17.000000 hapm-0.0.5/hapm.egg-info/top_level.txt
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-31 08:59:17.341959 hapm-0.0.5/libhapm/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)        0 2023-02-17 18:11:43.000000 hapm-0.0.5/libhapm/__init__.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-31 08:59:17.343880 hapm-0.0.5/libhapm/cli/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      184 2023-02-22 22:09:22.000000 hapm-0.0.5/libhapm/cli/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      390 2023-02-22 19:26:44.000000 hapm-0.0.5/libhapm/cli/ink.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1314 2023-02-25 20:31:31.000000 hapm-0.0.5/libhapm/cli/report_diff.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      871 2023-02-25 20:31:45.000000 hapm-0.0.5/libhapm/cli/report_list.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      443 2023-02-22 22:14:02.000000 hapm-0.0.5/libhapm/cli/report_no_token.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      930 2023-02-22 20:03:50.000000 hapm-0.0.5/libhapm/cli/report_summary.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      637 2023-02-25 10:20:29.000000 hapm-0.0.5/libhapm/cli/utils.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-31 08:59:17.344748 hapm-0.0.5/libhapm/github/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      147 2023-02-25 20:18:07.000000 hapm-0.0.5/libhapm/github/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      871 2023-02-25 20:12:15.000000 hapm-0.0.5/libhapm/github/file.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      325 2023-02-25 20:17:01.000000 hapm-0.0.5/libhapm/github/path.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      422 2023-02-25 20:18:42.000000 hapm-0.0.5/libhapm/github/tarball.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-31 08:59:17.345340 hapm-0.0.5/libhapm/integration/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       71 2023-02-25 10:15:54.000000 hapm-0.0.5/libhapm/integration/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     2142 2023-02-26 16:02:42.000000 hapm-0.0.5/libhapm/integration/package.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-31 08:59:17.345972 hapm-0.0.5/libhapm/manager/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     5144 2023-02-26 16:07:00.000000 hapm-0.0.5/libhapm/manager/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      301 2023-02-22 12:53:26.000000 hapm-0.0.5/libhapm/manager/diff.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      985 2023-02-21 10:33:48.000000 hapm-0.0.5/libhapm/manager/lockfile.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-31 08:59:17.346825 hapm-0.0.5/libhapm/manifest/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       31 2023-02-20 20:36:51.000000 hapm-0.0.5/libhapm/manifest/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      692 2023-02-22 19:17:05.000000 hapm-0.0.5/libhapm/manifest/manifest.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1107 2023-02-25 11:28:23.000000 hapm-0.0.5/libhapm/manifest/parse.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-31 08:59:17.347436 hapm-0.0.5/libhapm/package/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      101 2023-02-25 20:13:51.000000 hapm-0.0.5/libhapm/package/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     2342 2023-02-26 15:43:41.000000 hapm-0.0.5/libhapm/package/base.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      210 2023-02-25 10:18:53.000000 hapm-0.0.5/libhapm/package/description.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-31 08:59:17.347844 hapm-0.0.5/libhapm/plugin/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       34 2023-02-25 20:29:49.000000 hapm-0.0.5/libhapm/plugin/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     2613 2023-02-26 16:07:40.000000 hapm-0.0.5/libhapm/plugin/package.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      961 2023-02-20 20:57:56.000000 hapm-0.0.5/libhapm/versions.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      397 2023-02-20 20:34:09.000000 hapm-0.0.5/pyproject.toml
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-31 08:59:17.349135 hapm-0.0.5/scripts/
+-rwxr-xr-x   0 mishamyrt   (501) staff       (20)     1954 2023-02-26 15:42:57.000000 hapm-0.0.5/scripts/hapm
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       38 2023-07-31 08:59:17.349578 hapm-0.0.5/setup.cfg
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1062 2023-02-25 20:30:08.000000 hapm-0.0.5/setup.py
```

### Comparing `hapm-0.0.4/PKG-INFO` & `hapm-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hapm
-Version: 0.0.4
+Version: 0.0.5
 Summary: The library for easily writing feature-rich Python scripts
 Home-page: UNKNOWN
 Author: Mikhael Khrustik
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -60,21 +60,15 @@
 
 **not yet implemented**
 
 ```sh
 hapm get -t integration https://github.com/AlexxIT/XiaomiGateway3
 ```
 
-## Update
-
-**not yet implemented**
+## Updates
 
 ```sh
-# Update all packages to latest version
-hapm update
-# Update all packages to latest version
-hapm update <url>
-# Only print
-hapm update --dry
+# Prints updates
+hapm updates
 ```
```

### Comparing `hapm-0.0.4/README.md` & `hapm-0.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -47,19 +47,13 @@
 
 **not yet implemented**
 
 ```sh
 hapm get -t integration https://github.com/AlexxIT/XiaomiGateway3
 ```
 
-## Update
-
-**not yet implemented**
+## Updates
 
 ```sh
-# Update all packages to latest version
-hapm update
-# Update all packages to latest version
-hapm update <url>
-# Only print
-hapm update --dry
+# Prints updates
+hapm updates
 ```
```

### Comparing `hapm-0.0.4/hapm.egg-info/PKG-INFO` & `hapm-0.0.5/hapm.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hapm
-Version: 0.0.4
+Version: 0.0.5
 Summary: The library for easily writing feature-rich Python scripts
 Home-page: UNKNOWN
 Author: Mikhael Khrustik
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -60,21 +60,15 @@
 
 **not yet implemented**
 
 ```sh
 hapm get -t integration https://github.com/AlexxIT/XiaomiGateway3
 ```
 
-## Update
-
-**not yet implemented**
+## Updates
 
 ```sh
-# Update all packages to latest version
-hapm update
-# Update all packages to latest version
-hapm update <url>
-# Only print
-hapm update --dry
+# Prints updates
+hapm updates
 ```
```

### Comparing `hapm-0.0.4/libhapm/versions.py` & `hapm-0.0.5/libhapm/versions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Вспомогательные функции для работы с версиями"""
 from re import match
+from typing import List
+
 from pkg_resources import parse_version
 
 STABLE_VERSION_RE = r'^v?\d+\.\d+(\.\d+)?$'
 
-def find_latest_stable(tags: dict) -> str:
+def find_latest_stable(tags: List[str]) -> str:
     """Находит последнюю стабильную версию в списке"""
     latest = '0.0.0'
     for tag in tags:
         if not is_stable(tag):
             continue
         if is_newer(latest, tag):
             latest = tag
```

### Comparing `hapm-0.0.4/setup.py` & `hapm-0.0.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,25 +12,30 @@
     version=VERSION,
     author="Mikhael Khrustik",
     description="The library for easily writing feature-rich Python scripts",
     long_description=README,
     long_description_content_type="text/markdown",
     packages=[
         'libhapm',
-        'libhapm.integrations',
-        'libhapm.packages',
-        'libhapm.packages.manifest',
-        'libhapm.repository',
+        'libhapm.cli',
+        'libhapm.github',
+        'libhapm.integration',
+        'libhapm.package',
+        'libhapm.manager',
+        'libhapm.plugin',
+        'libhapm.manifest',
     ],
     scripts=['scripts/hapm'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License"
     ],
     install_requires=[
         'ruamel.yaml==0.17.21',
         'arrrgs==0.0.5',
-        'gitpython==3.1.30'
+        'gitpython==3.1.30',
+        'PyGithub==1.58.0',
+        'requests'
     ],
     python_requires='>=3.7',
     package_dir={'': '.'},
 )
```

