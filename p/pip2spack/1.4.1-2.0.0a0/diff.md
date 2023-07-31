# Comparing `tmp/pip2spack-1.4.1.tar.gz` & `tmp/pip2spack-2.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip2spack-1.4.1.tar", last modified: Thu Jul 21 18:45:21 2022, max compression
+gzip compressed data, was "pip2spack-2.0.0a0.tar", last modified: Mon Jul 31 11:42:59 2023, max compression
```

## Comparing `pip2spack-1.4.1.tar` & `pip2spack-2.0.0a0.tar`

### file list

```diff
@@ -1,56 +1,50 @@
-drwxr-xr-x   0 tomek      (501) staff       (20)        0 2022-07-21 18:45:21.844578 pip2spack-1.4.1/
--rw-r--r--   0 tomek      (501) staff       (20)     1066 2022-07-19 18:57:43.000000 pip2spack-1.4.1/LICENSE
--rw-r--r--   0 tomek      (501) staff       (20)     2543 2022-07-21 18:45:21.844286 pip2spack-1.4.1/PKG-INFO
--rw-r--r--   0 tomek      (501) staff       (20)     2026 2022-07-19 18:57:43.000000 pip2spack-1.4.1/README.md
-drwxr-xr-x   0 tomek      (501) staff       (20)        0 2022-07-21 18:45:21.839455 pip2spack-1.4.1/pip2spack/
--rw-r--r--   0 tomek      (501) staff       (20)        0 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/__init__.py
-drwxr-xr-x   0 tomek      (501) staff       (20)        0 2022-07-21 18:45:21.840695 pip2spack-1.4.1/pip2spack/actions/
--rw-r--r--   0 tomek      (501) staff       (20)        0 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/actions/__init__.py
--rw-r--r--   0 tomek      (501) staff       (20)      652 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/actions/action.py
--rw-r--r--   0 tomek      (501) staff       (20)     1363 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/actions/action_dispatcher.py
-drwxr-xr-x   0 tomek      (501) staff       (20)        0 2022-07-21 18:45:21.840952 pip2spack-1.4.1/pip2spack/actions/create/
--rw-r--r--   0 tomek      (501) staff       (20)        0 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/actions/create/__init__.py
--rw-r--r--   0 tomek      (501) staff       (20)     1367 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/actions/create/create_action.py
-drwxr-xr-x   0 tomek      (501) staff       (20)        0 2022-07-21 18:45:21.841166 pip2spack-1.4.1/pip2spack/actions/dowload/
--rw-r--r--   0 tomek      (501) staff       (20)        0 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/actions/dowload/__init__.py
--rw-r--r--   0 tomek      (501) staff       (20)      858 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/actions/dowload/download_action.py
-drwxr-xr-x   0 tomek      (501) staff       (20)        0 2022-07-21 18:45:21.841369 pip2spack-1.4.1/pip2spack/actions/update/
--rw-r--r--   0 tomek      (501) staff       (20)        0 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/actions/update/__init__.py
--rw-r--r--   0 tomek      (501) staff       (20)      901 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/actions/update/update_action.py
--rw-r--r--   0 tomek      (501) staff       (20)      262 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/actions/version.py
-drwxr-xr-x   0 tomek      (501) staff       (20)        0 2022-07-21 18:45:21.841944 pip2spack-1.4.1/pip2spack/core/
--rw-r--r--   0 tomek      (501) staff       (20)        0 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/core/__init__.py
--rw-r--r--   0 tomek      (501) staff       (20)     3900 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/core/package.py
--rw-r--r--   0 tomek      (501) staff       (20)     7267 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/core/pypi_package.py
--rw-r--r--   0 tomek      (501) staff       (20)     1874 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/core/spack_repository.py
--rw-r--r--   0 tomek      (501) staff       (20)     1215 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/core/verification.py
-drwxr-xr-x   0 tomek      (501) staff       (20)        0 2022-07-21 18:45:21.842346 pip2spack-1.4.1/pip2spack/framework/
--rw-r--r--   0 tomek      (501) staff       (20)        0 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/framework/__init__.py
--rw-r--r--   0 tomek      (501) staff       (20)      454 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/framework/constants.py
--rw-r--r--   0 tomek      (501) staff       (20)     1308 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/framework/helpers.py
--rw-r--r--   0 tomek      (501) staff       (20)      900 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/framework/messages.py
-drwxr-xr-x   0 tomek      (501) staff       (20)        0 2022-07-21 18:45:21.842566 pip2spack-1.4.1/pip2spack/main/
--rw-r--r--   0 tomek      (501) staff       (20)        0 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/main/__init__.py
--rw-r--r--   0 tomek      (501) staff       (20)      289 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/main/main.py
-drwxr-xr-x   0 tomek      (501) staff       (20)        0 2022-07-21 18:45:21.842754 pip2spack-1.4.1/pip2spack/templates/
--rw-r--r--   0 tomek      (501) staff       (20)        0 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/templates/__init__.py
--rw-r--r--   0 tomek      (501) staff       (20)      899 2022-07-20 19:02:56.000000 pip2spack-1.4.1/pip2spack/templates/package.j2
-drwxr-xr-x   0 tomek      (501) staff       (20)        0 2022-07-21 18:45:21.840136 pip2spack-1.4.1/pip2spack.egg-info/
--rw-r--r--   0 tomek      (501) staff       (20)     2543 2022-07-21 18:45:21.000000 pip2spack-1.4.1/pip2spack.egg-info/PKG-INFO
--rw-r--r--   0 tomek      (501) staff       (20)     1232 2022-07-21 18:45:21.000000 pip2spack-1.4.1/pip2spack.egg-info/SOURCES.txt
--rw-r--r--   0 tomek      (501) staff       (20)        1 2022-07-21 18:45:21.000000 pip2spack-1.4.1/pip2spack.egg-info/dependency_links.txt
--rw-r--r--   0 tomek      (501) staff       (20)       56 2022-07-21 18:45:21.000000 pip2spack-1.4.1/pip2spack.egg-info/entry_points.txt
--rw-r--r--   0 tomek      (501) staff       (20)       67 2022-07-21 18:45:21.000000 pip2spack-1.4.1/pip2spack.egg-info/requires.txt
--rw-r--r--   0 tomek      (501) staff       (20)       16 2022-07-21 18:45:21.000000 pip2spack-1.4.1/pip2spack.egg-info/top_level.txt
--rw-r--r--   0 tomek      (501) staff       (20)       38 2022-07-21 18:45:21.844647 pip2spack-1.4.1/setup.cfg
--rw-r--r--   0 tomek      (501) staff       (20)     1086 2022-07-20 19:02:56.000000 pip2spack-1.4.1/setup.py
-drwxr-xr-x   0 tomek      (501) staff       (20)        0 2022-07-21 18:45:21.842877 pip2spack-1.4.1/tests/
--rw-r--r--   0 tomek      (501) staff       (20)        0 2022-07-19 19:04:35.000000 pip2spack-1.4.1/tests/__init__.py
-drwxr-xr-x   0 tomek      (501) staff       (20)        0 2022-07-21 18:45:21.842962 pip2spack-1.4.1/tests/pip2spack/
--rw-r--r--   0 tomek      (501) staff       (20)        0 2022-07-19 19:04:41.000000 pip2spack-1.4.1/tests/pip2spack/__init__.py
-drwxr-xr-x   0 tomek      (501) staff       (20)        0 2022-07-21 18:45:21.844001 pip2spack-1.4.1/tests/pip2spack/core/
--rw-r--r--   0 tomek      (501) staff       (20)        0 2022-07-19 19:04:48.000000 pip2spack-1.4.1/tests/pip2spack/core/__init__.py
--rw-r--r--   0 tomek      (501) staff       (20)      908 2022-07-20 19:02:56.000000 pip2spack-1.4.1/tests/pip2spack/core/conftest.py
--rw-r--r--   0 tomek      (501) staff       (20)   183252 2022-07-20 19:02:56.000000 pip2spack-1.4.1/tests/pip2spack/core/mocks.py
--rw-r--r--   0 tomek      (501) staff       (20)     1827 2022-07-20 19:02:56.000000 pip2spack-1.4.1/tests/pip2spack/core/test_pypi_package.py
--rw-r--r--   0 tomek      (501) staff       (20)     1543 2022-07-21 18:44:27.000000 pip2spack-1.4.1/tests/pip2spack/core/test_verification.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:42:59.159621 pip2spack-2.0.0a0/
+-rw-rw-rw-   0        0        0     1087 2023-07-30 08:33:42.000000 pip2spack-2.0.0a0/LICENSE
+-rw-rw-rw-   0        0        0     2609 2023-07-31 11:42:59.158620 pip2spack-2.0.0a0/PKG-INFO
+-rw-rw-rw-   0        0        0     2113 2023-07-30 08:33:42.000000 pip2spack-2.0.0a0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 11:42:59.121951 pip2spack-2.0.0a0/pip2spack/
+-rw-rw-rw-   0        0        0        0 2023-07-30 08:33:42.000000 pip2spack-2.0.0a0/pip2spack/__init__.py
+-rw-rw-rw-   0        0        0     1056 2023-07-31 10:18:19.000000 pip2spack-2.0.0a0/pip2spack/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:42:59.129951 pip2spack-2.0.0a0/pip2spack/actions/
+-rw-rw-rw-   0        0        0        0 2023-07-30 08:33:42.000000 pip2spack-2.0.0a0/pip2spack/actions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:42:59.131952 pip2spack-2.0.0a0/pip2spack/actions/create/
+-rw-rw-rw-   0        0        0        0 2023-07-30 08:33:42.000000 pip2spack-2.0.0a0/pip2spack/actions/create/__init__.py
+-rw-rw-rw-   0        0        0      962 2023-07-31 09:57:07.000000 pip2spack-2.0.0a0/pip2spack/actions/create/create_action.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:42:59.133952 pip2spack-2.0.0a0/pip2spack/actions/dowload/
+-rw-rw-rw-   0        0        0        0 2023-07-30 08:33:42.000000 pip2spack-2.0.0a0/pip2spack/actions/dowload/__init__.py
+-rw-rw-rw-   0        0        0      543 2023-07-31 10:04:39.000000 pip2spack-2.0.0a0/pip2spack/actions/dowload/download_action.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:42:59.137951 pip2spack-2.0.0a0/pip2spack/actions/update/
+-rw-rw-rw-   0        0        0        0 2023-07-30 08:33:42.000000 pip2spack-2.0.0a0/pip2spack/actions/update/__init__.py
+-rw-rw-rw-   0        0        0      517 2023-07-31 09:50:22.000000 pip2spack-2.0.0a0/pip2spack/actions/update/update_action.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:42:59.144610 pip2spack-2.0.0a0/pip2spack/core/
+-rw-rw-rw-   0        0        0        0 2023-07-30 08:33:42.000000 pip2spack-2.0.0a0/pip2spack/core/__init__.py
+-rw-rw-rw-   0        0        0     4143 2023-07-31 10:01:30.000000 pip2spack-2.0.0a0/pip2spack/core/package.py
+-rw-rw-rw-   0        0        0     7471 2023-07-31 09:47:43.000000 pip2spack-2.0.0a0/pip2spack/core/pypi_package.py
+-rw-rw-rw-   0        0        0     1931 2023-07-30 08:33:42.000000 pip2spack-2.0.0a0/pip2spack/core/spack_repository.py
+-rw-rw-rw-   0        0        0     1280 2023-07-31 09:49:42.000000 pip2spack-2.0.0a0/pip2spack/core/verification.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:42:59.148624 pip2spack-2.0.0a0/pip2spack/framework/
+-rw-rw-rw-   0        0        0        0 2023-07-30 08:33:42.000000 pip2spack-2.0.0a0/pip2spack/framework/__init__.py
+-rw-rw-rw-   0        0        0      468 2023-07-30 08:33:42.000000 pip2spack-2.0.0a0/pip2spack/framework/constants.py
+-rw-rw-rw-   0        0        0     1358 2023-07-31 09:53:00.000000 pip2spack-2.0.0a0/pip2spack/framework/helpers.py
+-rw-rw-rw-   0        0        0      968 2023-07-31 09:48:56.000000 pip2spack-2.0.0a0/pip2spack/framework/messages.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:42:59.150621 pip2spack-2.0.0a0/pip2spack/templates/
+-rw-rw-rw-   0        0        0        0 2023-07-30 08:33:42.000000 pip2spack-2.0.0a0/pip2spack/templates/__init__.py
+-rw-rw-rw-   0        0        0      930 2023-07-30 08:33:42.000000 pip2spack-2.0.0a0/pip2spack/templates/package.j2
+drwxrwxrwx   0        0        0        0 2023-07-31 11:42:59.128950 pip2spack-2.0.0a0/pip2spack.egg-info/
+-rw-rw-rw-   0        0        0     2609 2023-07-31 11:42:59.000000 pip2spack-2.0.0a0/pip2spack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1066 2023-07-31 11:42:59.000000 pip2spack-2.0.0a0/pip2spack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 11:42:59.000000 pip2spack-2.0.0a0/pip2spack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-07-31 11:42:59.000000 pip2spack-2.0.0a0/pip2spack.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       80 2023-07-31 11:42:59.000000 pip2spack-2.0.0a0/pip2spack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-31 11:42:59.000000 pip2spack-2.0.0a0/pip2spack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 11:42:59.159621 pip2spack-2.0.0a0/setup.cfg
+-rw-rw-rw-   0        0        0     1040 2023-07-31 10:17:27.000000 pip2spack-2.0.0a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:42:59.152624 pip2spack-2.0.0a0/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-30 08:33:42.000000 pip2spack-2.0.0a0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:42:59.153647 pip2spack-2.0.0a0/tests/pip2spack/
+-rw-rw-rw-   0        0        0        0 2023-07-30 08:33:42.000000 pip2spack-2.0.0a0/tests/pip2spack/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:42:59.157620 pip2spack-2.0.0a0/tests/pip2spack/core/
+-rw-rw-rw-   0        0        0        0 2023-07-30 08:33:42.000000 pip2spack-2.0.0a0/tests/pip2spack/core/__init__.py
+-rw-rw-rw-   0        0        0      940 2023-07-30 08:33:42.000000 pip2spack-2.0.0a0/tests/pip2spack/core/conftest.py
+-rw-rw-rw-   0        0        0   186861 2023-07-30 08:33:42.000000 pip2spack-2.0.0a0/tests/pip2spack/core/mocks.py
+-rw-rw-rw-   0        0        0     1875 2023-07-30 08:33:42.000000 pip2spack-2.0.0a0/tests/pip2spack/core/test_pypi_package.py
```

### Comparing `pip2spack-1.4.1/PKG-INFO` & `pip2spack-2.0.0a0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,105 +1,101 @@
-Metadata-Version: 2.1
-Name: pip2spack
-Version: 1.4.1
-Summary: Automatically create and update a spack package base on the pypi.org information
-Home-page: https://github.com/NexSabre/pip2spack
-Author: Nex Sabre
-Author-email: nexsabre@protonmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pip2Spack
-![Test](https://github.com/NexSabre/pip2spack/workflows/Test/badge.svg?branch=master)
-[![PyPI version](https://badge.fury.io/py/pip2spack.svg)](https://badge.fury.io/py/pip2spack)
-
-Automatically create and update a spack package base on the pypi.org information.
-
-__Cons__:
- - Faster package creation than using the default option `spack create`
- - Automatic updating of existing packages with information contained on pypi.org
- 
- 
-## TL;DR
-```
-// install 
-pip install pip2spack 
-
-// create new one
-pip2spack create jsl
-
-// update a internal (bultin) package
-pip2spack update codecov 
-
-// download latest package locally 
-pip2spack download jsl codecov
-```
-
-
-## Installation
-Later, the package will be added into pypi repository.
-```
-pip install pip2spack
-```
-
-## Build
-To build a .whl package
-
-```
-pip install setuptools wheel twine
-python setup.py sdist bdist_wheel
-```
-
-Than go to `dist` directory and type
-
-```
-pip install pip2spack-1.0-py3-none-any.whl
-```
-
-## Run
-Before you run the script download a spack and export `SPACK_ROOT`. 
-### Create a new package
-To run a script, provide a package names:
-```
-pip2spack create {package_names_for_convert}
-```
-
-Example for creation one new package:
-```
-pip2spack create jsl 
-```
-
-you can also create more than one in single run:
-```
-pip2spack create jsl codecov
-```
-
-### Updating existing packages (builtin)
-Since v0.2, pip2spack is able to update builtin packages to newest version base on the pypi.org information.
-
-__No more adding a new version thru Spack's Pull Requests!__ 
-
-Example:
-```
-pip2spack update codecov
-```
-
-__Notice:__ You can not to create and update packages at once. These operations are separated (in actual version)
-
-
-### Downloading a newest packages locally
-Since v1.1, pip2spack is able to download latest `.tar.gz`/`.whl` package locally, using `download` command
-
-Example:
-```
-pip2spack download jsl codecov
-```
-
-Packages will be stored at the `temp` directory (depends on the OS), proper information wit storage place will be displayed.
-
-
+Metadata-Version: 2.1
+Name: pip2spack
+Version: 2.0.0a0
+Summary: Automatically create and update a spack package base on the pypi.org information
+Home-page: https://github.com/NexSabre/pip2spack
+Author: Nex Sabre
+Author-email: nexsabre@protonmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pip2Spack
+![Test](https://github.com/NexSabre/pip2spack/workflows/Test/badge.svg?branch=master)
+[![PyPI version](https://badge.fury.io/py/pip2spack.svg)](https://badge.fury.io/py/pip2spack)
+
+Automatically create and update a spack package base on the pypi.org information.
+
+__Cons__:
+ - Faster package creation than using the default option `spack create`
+ - Automatic updating of existing packages with information contained on pypi.org
+ 
+ 
+## TL;DR
+```
+// install 
+pip install pip2spack 
+
+// create new one
+pip2spack create jsl
+
+// update a internal (bultin) package
+pip2spack update codecov 
+
+// download latest package locally 
+pip2spack download jsl codecov
+```
+
+
+## Installation
+Later, the package will be added into pypi repository.
+```
+pip install pip2spack
+```
+
+## Build
+To build a .whl package
+
+```
+pip install setuptools wheel twine
+python setup.py sdist bdist_wheel
+```
+
+Than go to `dist` directory and type
+
+```
+pip install pip2spack-1.0-py3-none-any.whl
+```
+
+## Run
+Before you run the script download a spack and export `SPACK_ROOT`. 
+### Create a new package
+To run a script, provide a package names:
+```
+pip2spack create {package_names_for_convert}
+```
+
+Example for creation one new package:
+```
+pip2spack create jsl 
+```
+
+you can also create more than one in single run:
+```
+pip2spack create jsl codecov
+```
+
+### Updating existing packages (builtin)
+Since v0.2, pip2spack is able to update builtin packages to newest version base on the pypi.org information.
+
+__No more adding a new version thru Spack's Pull Requests!__ 
+
+Example:
+```
+pip2spack update codecov
+```
+
+__Notice:__ You can not to create and update packages at once. These operations are separated (in actual version)
+
+
+### Downloading a newest packages locally
+Since v1.1, pip2spack is able to download latest `.tar.gz`/`.whl` package locally, using `download` command
+
+Example:
+```
+pip2spack download jsl codecov
+```
+
+Packages will be stored at the `temp` directory (depends on the OS), proper information wit storage place will be displayed.
```

### Comparing `pip2spack-1.4.1/README.md` & `pip2spack-2.0.0a0/README.md`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-# pip2Spack
-![Test](https://github.com/NexSabre/pip2spack/workflows/Test/badge.svg?branch=master)
-[![PyPI version](https://badge.fury.io/py/pip2spack.svg)](https://badge.fury.io/py/pip2spack)
-
-Automatically create and update a spack package base on the pypi.org information.
-
-__Cons__:
- - Faster package creation than using the default option `spack create`
- - Automatic updating of existing packages with information contained on pypi.org
- 
- 
-## TL;DR
-```
-// install 
-pip install pip2spack 
-
-// create new one
-pip2spack create jsl
-
-// update a internal (bultin) package
-pip2spack update codecov 
-
-// download latest package locally 
-pip2spack download jsl codecov
-```
-
-
-## Installation
-Later, the package will be added into pypi repository.
-```
-pip install pip2spack
-```
-
-## Build
-To build a .whl package
-
-```
-pip install setuptools wheel twine
-python setup.py sdist bdist_wheel
-```
-
-Than go to `dist` directory and type
-
-```
-pip install pip2spack-1.0-py3-none-any.whl
-```
-
-## Run
-Before you run the script download a spack and export `SPACK_ROOT`. 
-### Create a new package
-To run a script, provide a package names:
-```
-pip2spack create {package_names_for_convert}
-```
-
-Example for creation one new package:
-```
-pip2spack create jsl 
-```
-
-you can also create more than one in single run:
-```
-pip2spack create jsl codecov
-```
-
-### Updating existing packages (builtin)
-Since v0.2, pip2spack is able to update builtin packages to newest version base on the pypi.org information.
-
-__No more adding a new version thru Spack's Pull Requests!__ 
-
-Example:
-```
-pip2spack update codecov
-```
-
-__Notice:__ You can not to create and update packages at once. These operations are separated (in actual version)
-
-
-### Downloading a newest packages locally
-Since v1.1, pip2spack is able to download latest `.tar.gz`/`.whl` package locally, using `download` command
-
-Example:
-```
-pip2spack download jsl codecov
-```
-
-Packages will be stored at the `temp` directory (depends on the OS), proper information wit storage place will be displayed.
+# pip2Spack
+![Test](https://github.com/NexSabre/pip2spack/workflows/Test/badge.svg?branch=master)
+[![PyPI version](https://badge.fury.io/py/pip2spack.svg)](https://badge.fury.io/py/pip2spack)
+
+Automatically create and update a spack package base on the pypi.org information.
+
+__Cons__:
+ - Faster package creation than using the default option `spack create`
+ - Automatic updating of existing packages with information contained on pypi.org
+ 
+ 
+## TL;DR
+```
+// install 
+pip install pip2spack 
+
+// create new one
+pip2spack create jsl
+
+// update a internal (bultin) package
+pip2spack update codecov 
+
+// download latest package locally 
+pip2spack download jsl codecov
+```
+
+
+## Installation
+Later, the package will be added into pypi repository.
+```
+pip install pip2spack
+```
+
+## Build
+To build a .whl package
+
+```
+pip install setuptools wheel twine
+python setup.py sdist bdist_wheel
+```
+
+Than go to `dist` directory and type
+
+```
+pip install pip2spack-1.0-py3-none-any.whl
+```
+
+## Run
+Before you run the script download a spack and export `SPACK_ROOT`. 
+### Create a new package
+To run a script, provide a package names:
+```
+pip2spack create {package_names_for_convert}
+```
+
+Example for creation one new package:
+```
+pip2spack create jsl 
+```
+
+you can also create more than one in single run:
+```
+pip2spack create jsl codecov
+```
+
+### Updating existing packages (builtin)
+Since v0.2, pip2spack is able to update builtin packages to newest version base on the pypi.org information.
+
+__No more adding a new version thru Spack's Pull Requests!__ 
+
+Example:
+```
+pip2spack update codecov
+```
+
+__Notice:__ You can not to create and update packages at once. These operations are separated (in actual version)
+
+
+### Downloading a newest packages locally
+Since v1.1, pip2spack is able to download latest `.tar.gz`/`.whl` package locally, using `download` command
+
+Example:
+```
+pip2spack download jsl codecov
+```
+
+Packages will be stored at the `temp` directory (depends on the OS), proper information wit storage place will be displayed.
```

### Comparing `pip2spack-1.4.1/pip2spack/core/package.py` & `pip2spack-2.0.0a0/pip2spack/core/package.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,107 +1,108 @@
-import os
-from dataclasses import dataclass
-
-from pip2spack.core.pypi_package import PyPiPackage
-from pip2spack.core.spack_repository import SpackRepository
-from pip2spack.framework import constants as constants
-from pip2spack.framework.messages import Messages
-
-
-@dataclass
-class Package:
-    package_name: str
-    package_path: str
-    _raw_package: str
-
-    versions: list
-    modification_package: list
-
-    def __post_init__(self):
-        self.package_path = SpackRepository().get_package_path(
-            package_name=self.package_name
-        )
-        self._open()
-
-    def _open(self):
-        with open(self.package_path, "r") as package_py:
-            self._raw_package = package_py.read()
-
-    def replace_structure_with_marker(self):
-        self.modification_package = self._raw_package.split("\n")
-        if not isinstance(self.modification_package, list):
-            raise
-
-        rows_with_version = []
-        for index, content in enumerate(self.modification_package):
-            if "version(" in content:
-                rows_with_version.append((index, content.lstrip().rstrip()))
-
-        rows_with_version.reverse()  # start removing an empty rows from bottom file
-        for index, row in enumerate(rows_with_version):
-            if index == 0:
-                self.modification_package[row[0]] = self.modification_package[
-                    row[0]
-                ].replace(row[1], constants.MARKER_VERSION)
-            else:
-                del self.modification_package[row[0]]
-
-        self.replace_marker_with_template()
-
-    def replace_marker_with_template(self):
-        rows_with_version = []
-        for index, content in enumerate(self.modification_package):
-            if constants.MARKER_VERSION in content:
-                rows_with_version.append(index)
-
-        if not [x for x in self.modification_package if constants.MARKER_VERSION in x]:
-            Messages.error(
-                f"{self.package_name} :: pip2spack can not find a 'version' tag.\n\t"
-                f" Please create a new package with:\n\t"
-                f"  pip2spack create {self.package_name}"
-            )
-            return
-
-        rows_with_version.reverse()  # start removing an empty rows from bottom file
-        for index, row in enumerate(rows_with_version):
-            if index == 0:
-                spaces = self._count_trailing_spaces(self.modification_package[row])
-                self.modification_package[row] = self.modification_package[row].replace(
-                    constants.MARKER_VERSION, constants.marker_version_template(spaces)
-                )
-            else:
-                break
-
-        self.generate_modded_package(save=True)
-        if not self.save(self.update_newest_versions(self.package_name)):
-            Messages.error(
-                f"Something went wrong, package {self.package_name} was not updated"
-            )
-        else:
-            Messages.ok(
-                f"{self.package_name} :: builtin package was updated at {self.package_path}"
-            )
-
-    def update_newest_versions(self, package_name):
-        sp = PyPiPackage(package_name)
-        file = sp.generate_custom_file(
-            os.path.dirname(os.path.realpath(self.package_path)), sp._get_versions
-        )
-        return file
-
-    def save(self, new_file):
-        with open(self.package_path, "w") as package:
-            package.write(new_file)
-            return True
-
-    def generate_modded_package(self, save: bool = False):
-        if not save:
-            return "\n".join(self.modification_package).lstrip()
-        self.save("\n".join(self.modification_package).lstrip())
-
-    @staticmethod
-    def available_markers(marker_name):
-        return {"version": constants.MARKER_VERSION}.get(marker_name, None)
-
-    @staticmethod
-    def _count_trailing_spaces(sentence) -> int:
-        return len(sentence) - len(sentence.lstrip())
+import os
+from dataclasses import dataclass, field
+from typing import List, Optional
+
+from pip2spack.core.pypi_package import PyPiPackage
+from pip2spack.core.spack_repository import SpackRepository
+from pip2spack.framework import constants as constants
+from pip2spack.framework.messages import Messages
+
+
+@dataclass
+class Package:
+    package_name: str
+    package_path: Optional[str] = None
+    _raw_package: Optional[str] = None
+
+    versions: List = field(default_factory=list)
+    modification_package: List = field(default_factory=list)
+
+    def __post_init__(self):
+        self.package_path = SpackRepository().get_package_path(
+            package_name=self.package_name
+        )
+        self._open()
+
+    def _open(self):
+        with open(self.package_path, "r") as package_py:
+            self._raw_package = package_py.read()
+
+    def replace_structure_with_marker(self):
+        self.modification_package = self._raw_package.split("\n")
+        if not isinstance(self.modification_package, list):
+            raise
+
+        rows_with_version = []
+        for index, content in enumerate(self.modification_package):
+            if "version(" in content:
+                rows_with_version.append((index, content.lstrip().rstrip()))
+
+        rows_with_version.reverse()  # start removing an empty rows from bottom file
+        for index, row in enumerate(rows_with_version):
+            if index == 0:
+                self.modification_package[row[0]] = self.modification_package[
+                    row[0]
+                ].replace(row[1], constants.MARKER_VERSION)
+            else:
+                del self.modification_package[row[0]]
+
+        self.replace_marker_with_template()
+
+    def replace_marker_with_template(self):
+        rows_with_version = []
+        for index, content in enumerate(self.modification_package):
+            if constants.MARKER_VERSION in content:
+                rows_with_version.append(index)
+
+        if not [x for x in self.modification_package if constants.MARKER_VERSION in x]:
+            Messages.error(
+                f"{self.package_name} :: pip2spack can not find a 'version' tag.\n\t"
+                f" Please create a new package with:\n\t"
+                f"  pip2spack create {self.package_name}"
+            )
+            return
+
+        rows_with_version.reverse()  # start removing an empty rows from bottom file
+        for index, row in enumerate(rows_with_version):
+            if index == 0:
+                spaces = self._count_trailing_spaces(self.modification_package[row])
+                self.modification_package[row] = self.modification_package[row].replace(
+                    constants.MARKER_VERSION, constants.marker_version_template(spaces)
+                )
+            else:
+                break
+
+        self.generate_modded_package(save=True)
+        if not self.save(self.update_newest_versions(self.package_name)):
+            Messages.error(
+                f"Something went wrong, package {self.package_name} was not updated"
+            )
+        else:
+            Messages.ok(
+                f"{self.package_name} :: builtin package was updated at {self.package_path}"
+            )
+
+    def update_newest_versions(self, package_name):
+        sp = PyPiPackage(package_name)
+        file = sp.generate_custom_file(
+            os.path.dirname(os.path.realpath(self.package_path)), sp._get_versions
+        )
+        return file
+
+    def save(self, new_file):
+        with open(self.package_path, "w") as package:
+            package.write(new_file)
+            return True
+
+    def generate_modded_package(self, save: bool = False):
+        if not save:
+            return "\n".join(self.modification_package).lstrip()
+        self.save("\n".join(self.modification_package).lstrip())
+
+    @staticmethod
+    def available_markers(marker_name):
+        return {"version": constants.MARKER_VERSION}.get(marker_name, None)
+
+    @staticmethod
+    def _count_trailing_spaces(sentence) -> int:
+        return len(sentence) - len(sentence.lstrip())
```

### Comparing `pip2spack-1.4.1/pip2spack/core/pypi_package.py` & `pip2spack-2.0.0a0/pip2spack/core/pypi_package.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,204 +1,204 @@
-import json
-from typing import Any, Dict, List
-
-import requests
-from jinja2 import Environment, FileSystemLoader, PackageLoader
-
-from pip2spack.framework.messages import Messages
-
-
-class PyPiPackage:
-    content: dict = {}
-    versions: list = []
-    url: str = ""
-    homepage: str = ""
-    maintainers: list = []
-    package_name: str = ""
-    summary: str = ""
-    source: bool = False
-
-    def __init__(self, content):
-        self.content = self._download_missing_information(content)
-
-        self._url(source=self.__detect_approach())
-
-        if self.source:
-            self._versions_formatter()
-        else:
-            self._wheel_versions_formatter()
-        self.version_builder()
-
-        self.package_name_builder()
-        self.summary_builder()
-        self.homepage_builder()
-
-    @property
-    def _get_versions(self):
-        self.versions = []
-        self._versions_formatter()
-        self.version_builder()
-        return self.versions
-
-    def __detect_approach(self) -> bool:
-        return True if self.content["urls"][0]["url"].endswith(".tar.gz") else False
-
-    @staticmethod
-    def _download_missing_information(package_name: str) -> Dict[str, Any]:
-        if package_name.startswith("py-"):
-            package_name = package_name.replace("py-", "")
-        status = requests.get(f"https://pypi.org/pypi/{package_name}/json")
-        if status.status_code != 200:
-            print("Package doesnt not exist at PyPi.org")
-            raise
-        return json.loads(status.content)
-
-    def _url(self, source):
-        def _generate_pypi_uri(filename_with_version):
-            if not filename_with_version:
-                raise Exception("Can not generate a proper master link to the package")
-            return (
-                f"https://pypi.io/packages/source/{filename_with_version[0]}/"
-                f'{"-".join(filename_with_version.split("-")[:-1])}/{filename_with_version}'
-            )
-
-        if source:
-            for url in self.content["urls"]:
-                if url["url"].endswith(".tar.gz"):
-                    self.url = _generate_pypi_uri(url["url"].split("/")[-1])
-                    self.source = True
-                    break
-        else:
-            # preferable packages are .tar.gz, but some author does not include it, they just provide .whl package
-            for u in self.content["urls"]:
-                if u["url"].endswith(".whl"):
-                    self.url = u["url"]
-                    self.source = False
-                    break
-
-        if not self.url:
-            raise Exception("Source package was not found")
-
-        elif self.url and not self.source:
-            print("[Experimental] Using a wheel package...")
-
-    def _homepage(self):
-        self.homepage = self.content["home_page"]
-
-    def _versions_formatter(self):
-        for version, version_content in self.content["releases"].items():
-            only_sdist_version = [
-                x
-                for x in version_content
-                if (x["url"].endswith(".tar.gz") and x["packagetype"] == "sdist")
-            ]
-            if not only_sdist_version:
-                continue
-
-            for proper_version in only_sdist_version:
-                try:
-                    # TODO Not support .whl packages yet. Only source code in .tar.gz
-                    if not proper_version["filename"].endswith(".tar.gz"):
-                        continue
-                    self.versions.append(
-                        (str(version), str(proper_version["digests"]["sha256"]))
-                    )
-                except IndexError:
-                    continue
-
-    def _wheel_versions_formatter(self):
-        # TODO: Experimental support of the .whl. It can be pulled out if creates more cons than props
-        for version, version_content in self.content["releases"].items():
-            only_bdist_wheel_version = [
-                x
-                for x in version_content
-                if (x["url"].endswith(".whl") and x["packagetype"] == "bdist_wheel")
-            ]
-
-            for proper_version in only_bdist_wheel_version:
-                try:
-                    if not proper_version["filename"].endswith(".whl"):
-                        continue
-                    self.versions.append(
-                        (str(version), str(proper_version["digests"]["sha256"]))
-                    )
-                except IndexError:
-                    continue
-
-    def version_builder(self) -> str:
-        raw_versions: str = ""
-        for v in self.versions:
-            raw_versions += f'version("{str(v[0])}", sha256="{str(v[1])}")\n'
-        return raw_versions
-
-    def package_name_builder(self) -> str:
-        name = self.content["info"]["name"]
-        if name[0].islower():
-            name = name[0].upper() + name[1:]
-
-        l_name = list(name)
-        for i in [index for index, element in enumerate(l_name) if element == "-"]:
-            try:
-                if l_name[i + 1].islower():
-                    l_name[i + 1] = l_name[i + 1].upper()
-            except Exception as e:
-                Messages.error(f"package_name_builder: {e}")
-            finally:
-                name = "".join(l_name).replace("-", "")
-
-        if not name.startswith("Py"):
-            name = "Py" + name
-        self.package_name = name
-        return name
-
-    def summary_builder(self):
-        self.summary = self.content["info"]["summary"]
-
-    def homepage_builder(self):
-        self.homepage = self.content["info"]["project_urls"]["Homepage"]
-
-    def _generate_data(self) -> dict:
-        return {
-            "package_name": self.package_name,
-            "summary": self.summary,
-            "homepage": self.homepage,
-            "url": self.url,
-            "versions": self.versions,
-            "depends_on_setuptools": False,
-        }
-
-    def generate_file(self):
-        env = Environment(loader=PackageLoader("pip2spack", "templates"))
-        template = env.get_template("package.j2")
-        return template.render(**self._generate_data())
-
-    @staticmethod
-    def generate_custom_file(abspath: str, versions):
-        env = Environment(loader=FileSystemLoader(abspath))
-        template = env.get_template("package.py")
-        return template.render({"versions": versions})
-
-    def download_versions(self, versions: List = None):
-        if not versions:
-            latest_version = self.content["info"]["version"]
-            latest_filename = self.content["releases"].get(latest_version)[0][
-                "filename"
-            ]
-            Messages.warn(
-                f"Missing versions parameter, downloading a latest one v{latest_version}"
-            )
-            r = requests.get(url=self.url)
-            self.__save_content(latest_filename, r.content)
-
-    @staticmethod
-    def __save_content(name: str, content: bytes):
-        import os
-        import tempfile
-
-        path = tempfile.gettempdir()
-        pip2spack = os.path.join(path, "pip2spack")
-        content_filename = os.path.join(pip2spack, name)
-        os.makedirs(pip2spack, exist_ok=True)
-
-        with open(content_filename, "wb") as content_to_save:
-            content_to_save.write(content)
-            Messages.info(f"Content was saved into {content_filename}")
+import json
+from typing import Any, Dict, List
+
+import requests
+from jinja2 import Environment, FileSystemLoader, PackageLoader
+
+from pip2spack.framework.messages import Messages
+
+
+class PyPiPackage:
+    content: Dict = {}
+    versions: List = []
+    url: str = ""
+    homepage: str = ""
+    maintainers: List = []
+    package_name: str = ""
+    summary: str = ""
+    source: bool = False
+
+    def __init__(self, content):
+        self.content = self._download_missing_information(content)
+
+        self._url(source=self.__detect_approach())
+
+        if self.source:
+            self._versions_formatter()
+        else:
+            self._wheel_versions_formatter()
+        self.version_builder()
+
+        self.package_name_builder()
+        self.summary_builder()
+        self.homepage_builder()
+
+    @property
+    def _get_versions(self):
+        self.versions = []
+        self._versions_formatter()
+        self.version_builder()
+        return self.versions
+
+    def __detect_approach(self) -> bool:
+        return True if self.content["urls"][0]["url"].endswith(".tar.gz") else False
+
+    @staticmethod
+    def _download_missing_information(package_name: str) -> Dict[str, Any]:
+        if package_name.startswith("py-"):
+            package_name = package_name.replace("py-", "")
+        status = requests.get(f"https://pypi.org/pypi/{package_name}/json")
+        if status.status_code != 200:
+            print("Package doesnt not exist at PyPi.org")
+            raise
+        return json.loads(status.content)
+
+    def _url(self, source):
+        def _generate_pypi_uri(filename_with_version):
+            if not filename_with_version:
+                raise Exception("Can not generate a proper master link to the package")
+            return (
+                f"https://pypi.io/packages/source/{filename_with_version[0]}/"
+                f'{"-".join(filename_with_version.split("-")[:-1])}/{filename_with_version}'
+            )
+
+        if source:
+            for url in self.content["urls"]:
+                if url["url"].endswith(".tar.gz"):
+                    self.url = _generate_pypi_uri(url["url"].split("/")[-1])
+                    self.source = True
+                    break
+        else:
+            # preferable packages are .tar.gz, but some author does not include it, they just provide .whl package
+            for u in self.content["urls"]:
+                if u["url"].endswith(".whl"):
+                    self.url = u["url"]
+                    self.source = False
+                    break
+
+        if not self.url:
+            raise Exception("Source package was not found")
+
+        elif self.url and not self.source:
+            print("[Experimental] Using a wheel package...")
+
+    def _homepage(self):
+        self.homepage = self.content["home_page"]
+
+    def _versions_formatter(self):
+        for version, version_content in self.content["releases"].items():
+            only_sdist_version = [
+                x
+                for x in version_content
+                if (x["url"].endswith(".tar.gz") and x["packagetype"] == "sdist")
+            ]
+            if not only_sdist_version:
+                continue
+
+            for proper_version in only_sdist_version:
+                try:
+                    # TODO Not support .whl packages yet. Only source code in .tar.gz
+                    if not proper_version["filename"].endswith(".tar.gz"):
+                        continue
+                    self.versions.append(
+                        (str(version), str(proper_version["digests"]["sha256"]))
+                    )
+                except IndexError:
+                    continue
+
+    def _wheel_versions_formatter(self):
+        # TODO: Experimental support of the .whl. It can be pulled out if creates more cons than props
+        for version, version_content in self.content["releases"].items():
+            only_bdist_wheel_version = [
+                x
+                for x in version_content
+                if (x["url"].endswith(".whl") and x["packagetype"] == "bdist_wheel")
+            ]
+
+            for proper_version in only_bdist_wheel_version:
+                try:
+                    if not proper_version["filename"].endswith(".whl"):
+                        continue
+                    self.versions.append(
+                        (str(version), str(proper_version["digests"]["sha256"]))
+                    )
+                except IndexError:
+                    continue
+
+    def version_builder(self) -> str:
+        raw_versions: str = ""
+        for v in self.versions:
+            raw_versions += f'version("{str(v[0])}", sha256="{str(v[1])}")\n'
+        return raw_versions
+
+    def package_name_builder(self) -> str:
+        name = self.content["info"]["name"]
+        if name[0].islower():
+            name = name[0].upper() + name[1:]
+
+        l_name = list(name)
+        for i in [index for index, element in enumerate(l_name) if element == "-"]:
+            try:
+                if l_name[i + 1].islower():
+                    l_name[i + 1] = l_name[i + 1].upper()
+            except Exception as e:
+                Messages.error(f"package_name_builder: {e}")
+            finally:
+                name = "".join(l_name).replace("-", "")
+
+        if not name.startswith("Py"):
+            name = "Py" + name
+        self.package_name = name
+        return name
+
+    def summary_builder(self):
+        self.summary = self.content["info"]["summary"]
+
+    def homepage_builder(self):
+        self.homepage = self.content["info"]["project_urls"]["Homepage"]
+
+    def _generate_data(self) -> dict:
+        return {
+            "package_name": self.package_name,
+            "summary": self.summary,
+            "homepage": self.homepage,
+            "url": self.url,
+            "versions": self.versions,
+            "depends_on_setuptools": False,
+        }
+
+    def generate_file(self):
+        env = Environment(loader=PackageLoader("pip2spack", "templates"))
+        template = env.get_template("package.j2")
+        return template.render(**self._generate_data())
+
+    @staticmethod
+    def generate_custom_file(abspath: str, versions):
+        env = Environment(loader=FileSystemLoader(abspath))
+        template = env.get_template("package.py")
+        return template.render({"versions": versions})
+
+    def download_versions(self, versions: List = None):
+        if not versions:
+            latest_version = self.content["info"]["version"]
+            latest_filename = self.content["releases"].get(latest_version)[0][
+                "filename"
+            ]
+            Messages.warn(
+                f"Missing versions parameter, downloading a latest one v{latest_version}"
+            )
+            r = requests.get(url=self.url)
+            self.__save_content(latest_filename, r.content)
+
+    @staticmethod
+    def __save_content(name: str, content: bytes):
+        import os
+        import tempfile
+
+        path = tempfile.gettempdir()
+        pip2spack = os.path.join(path, "pip2spack")
+        content_filename = os.path.join(pip2spack, name)
+        os.makedirs(pip2spack, exist_ok=True)
+
+        with open(content_filename, "wb") as content_to_save:
+            content_to_save.write(content)
+            Messages.info(f"Content was saved into {content_filename}")
```

### Comparing `pip2spack-1.4.1/pip2spack/core/spack_repository.py` & `pip2spack-2.0.0a0/pip2spack/core/spack_repository.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-from dataclasses import dataclass
-from os import getenv, listdir
-from os.path import abspath, exists, join, relpath
-
-from pip2spack.framework.constants import BUILTIN_REPOSITORY_REL_PATH
-from pip2spack.framework.messages import Messages
-
-
-@dataclass
-class SpackRepository:
-    _spack_root: str = getenv("SPACK_ROOT", "")
-    _builtin_repository: str = (
-        f"{join(_spack_root, relpath(BUILTIN_REPOSITORY_REL_PATH))}"
-        if _spack_root
-        else ""
-    )
-
-    @property
-    def directory(self):
-        return self._spack_root
-
-    @directory.setter
-    def directory(self, custom_spack_root):
-        if not exists(custom_spack_root):
-            raise
-        self._spack_root = custom_spack_root
-
-    @property
-    def builtin_repository(self):
-        return self._builtin_repository
-
-    def list_all_packages(self):
-        return listdir(self.builtin_repository)
-
-    def list_py_packages(self):
-        return [x for x in self.list_all_packages() if x.startswith("py-")]
-
-    def exists(self, package_name: str, python_only: bool = True) -> bool:
-        if python_only:
-            return package_name in self.list_py_packages()
-        else:
-            return package_name in self.list_all_packages()
-
-    def get_package_path(self, package_name: str) -> str:
-        """Return absolute path to the package.py if exists in builtin repository"""
-        if not package_name.startswith("py-"):
-            package_name = "py-" + package_name
-        package_py_path: str = join(
-            *(f"{self.builtin_repository}", package_name, "package.py")
-        )
-        if not self.exists(package_name) or not exists(package_py_path):
-            # TODO create a new one
-            Messages.warn(
-                f"Package {package_name} does not exist in the builtin repository"
-            )
-            raise
-        return abspath(package_py_path)
+from dataclasses import dataclass
+from os import getenv, listdir
+from os.path import abspath, exists, join, relpath
+
+from pip2spack.framework.constants import BUILTIN_REPOSITORY_REL_PATH
+from pip2spack.framework.messages import Messages
+
+
+@dataclass
+class SpackRepository:
+    _spack_root: str = getenv("SPACK_ROOT", "")
+    _builtin_repository: str = (
+        f"{join(_spack_root, relpath(BUILTIN_REPOSITORY_REL_PATH))}"
+        if _spack_root
+        else ""
+    )
+
+    @property
+    def directory(self):
+        return self._spack_root
+
+    @directory.setter
+    def directory(self, custom_spack_root):
+        if not exists(custom_spack_root):
+            raise
+        self._spack_root = custom_spack_root
+
+    @property
+    def builtin_repository(self):
+        return self._builtin_repository
+
+    def list_all_packages(self):
+        return listdir(self.builtin_repository)
+
+    def list_py_packages(self):
+        return [x for x in self.list_all_packages() if x.startswith("py-")]
+
+    def exists(self, package_name: str, python_only: bool = True) -> bool:
+        if python_only:
+            return package_name in self.list_py_packages()
+        else:
+            return package_name in self.list_all_packages()
+
+    def get_package_path(self, package_name: str) -> str:
+        """Return absolute path to the package.py if exists in builtin repository"""
+        if not package_name.startswith("py-"):
+            package_name = "py-" + package_name
+        package_py_path: str = join(
+            *(f"{self.builtin_repository}", package_name, "package.py")
+        )
+        if not self.exists(package_name) or not exists(package_py_path):
+            # TODO create a new one
+            Messages.warn(
+                f"Package {package_name} does not exist in the builtin repository"
+            )
+            raise
+        return abspath(package_py_path)
```

### Comparing `pip2spack-1.4.1/pip2spack/core/verification.py` & `pip2spack-2.0.0a0/pip2spack/core/verification.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-import json
-
-import requests
-
-from pip2spack.framework.messages import Messages
-
-
-class Verification:
-    def __init__(self, arguments: list):
-        self.__ready_packages = self.validate_pip_package_exists(arguments)
-        self.show_packages_for_process(self.__ready_packages, arguments)
-
-    @property
-    def available_packages(self):
-        return self.__ready_packages
-
-    @staticmethod
-    def validate_pip_package_exists(potential_packages):
-        if not potential_packages:
-            return
-
-        packages_status = {}
-        for package in potential_packages:
-            status = requests.get(f"https://pypi.org/pypi/{package}/json")
-            if status.status_code != 200:
-                continue
-            packages_status[package] = json.loads(status.content)
-        return packages_status
-
-    @staticmethod
-    def show_packages_for_process(package_ready, all_packages):
-        """Display at the terminal a information about arability of provided package names"""
-        packages_not_found = [x for x in all_packages if x not in package_ready]
-        packages_found = [k for k, v in package_ready.items()]
-        Messages.package_availability(packages_found, packages_not_found)
+import json
+from typing import List
+
+import requests
+
+from pip2spack.framework.messages import Messages
+
+
+class Verification:
+    def __init__(self, arguments: List[str]):
+        self.__ready_packages = self.validate_pip_package_exists(arguments)
+        self.show_packages_for_process(self.__ready_packages, arguments)
+
+    @property
+    def available_packages(self):
+        return self.__ready_packages
+
+    @staticmethod
+    def validate_pip_package_exists(potential_packages):
+        if not potential_packages:
+            return
+
+        packages_status = {}
+        for package in potential_packages:
+            status = requests.get(f"https://pypi.org/pypi/{package}/json")
+            if status.status_code != 200:
+                continue
+            packages_status[package] = json.loads(status.content)
+        return packages_status
+
+    @staticmethod
+    def show_packages_for_process(package_ready, all_packages):
+        """Display at the terminal a information about arability of provided package names"""
+        packages_not_found = [x for x in all_packages if x not in package_ready]
+        packages_found = [k for k, v in package_ready.items()]
+        Messages.package_availability(packages_found, packages_not_found)
```

### Comparing `pip2spack-1.4.1/pip2spack/framework/helpers.py` & `pip2spack-2.0.0a0/pip2spack/framework/helpers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import os
-
-
-def get_spack_repository() -> str:
-    """Return an absolute path about spack repository"""
-    spack_root = os.getenv("SPACK_ROOT", "")
-    if not spack_root:
-        print("Please provide a information about SPACK_ROOT")
-        exit(1)
-
-    repository_suburi = os.path.relpath("var/spack/repos/builtin/packages/")
-    repository_full_path = os.path.join(spack_root, repository_suburi)
-
-    if not os.path.exists(repository_full_path):
-        print("Spack repository does not exists")
-        exit(1)
-    return repository_full_path
-
-
-def create_directory(package_name):
-    """Create a package directory for the provided package name"""
-    if not package_name.startswith("py-"):
-        package_name = "py-" + package_name
-    target_path = os.path.join(get_spack_repository(), package_name)
-    if os.path.exists(target_path):
-        return False
-    try:
-        os.makedirs(target_path)
-    except FileExistsError:
-        pass
-    finally:
-        return os.path.exists(target_path)
-
-
-def create_package(name, raw) -> str:
-    if not name.startswith("py-"):
-        name = "py-" + name
-    target_path = os.path.join(get_spack_repository(), name)
-    with open(os.path.join(target_path, "package.py"), "w") as f:
-        f.write(raw)
-
-    return os.path.join(target_path, "package.py")
+import os
+
+
+def get_spack_repository() -> str:
+    """Return an absolute path about spack repository"""
+    spack_root = os.getenv("SPACK_ROOT", "")
+    if not spack_root:
+        print("Please provide a information about SPACK_ROOT")
+        exit(1)
+
+    repository_suburi = os.path.relpath("var/spack/repos/builtin/packages/")
+    repository_full_path = os.path.join(spack_root, repository_suburi)
+
+    if not os.path.exists(repository_full_path):
+        print("Spack repository does not exists")
+        exit(1)
+    return repository_full_path
+
+
+def create_directory(package_name) -> bool:
+    """Create a package directory for the provided package name"""
+    if not package_name.startswith("py-"):
+        package_name = "py-" + package_name
+    target_path = os.path.join(get_spack_repository(), package_name)
+    if os.path.exists(target_path):
+        return False
+    try:
+        os.makedirs(target_path)
+    except FileExistsError:
+        pass
+    finally:
+        return os.path.exists(target_path)
+
+
+def create_package(name, raw) -> str:
+    if not name.startswith("py-"):
+        name = "py-" + name
+    target_path = os.path.join(get_spack_repository(), name)
+    with open(os.path.join(target_path, "package.py"), "w") as f:
+        f.write(raw)
+
+    return os.path.join(target_path, "package.py")
```

### Comparing `pip2spack-1.4.1/pip2spack/templates/package.j2` & `pip2spack-2.0.0a0/pip2spack/templates/package.j2`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# Copyright 2013-2020 Lawrence Livermore National Security, LLC and other
-# Spack Project Developers. See the top-level COPYRIGHT file for details.
-#
-# SPDX-License-Identifier: (Apache-2.0 OR MIT)
-
-# Package automatically generated using 'pip2spack' converter
-
-
-class {{ package_name }}(PythonPackage):
-    """
-    {{ summary }}
-    """
-
-    homepage = "{{ homepage }}"
-    url      = "{{ url }}"
-
-    {% for v in versions|reverse %}
-    version('{{ v[0] }}', sha256='{{ v[1] }}'){% endfor %}
-
-    # depends_on('python@2.7:2.8,3.4:', type=('build', 'run'))
-    {% if depends_on_setuptools %}
-    depends_on('py-setuptools', type='build')
-    {% else %}
-    # depends_on('py-setuptools', type='build')
-    {% endif %}
-
-    def build_args(self, spec, prefix):
-        # FIXME: Add arguments other than --prefix
-        # FIXME: If not needed delete this function
-        args = []
-        return args
+# Copyright 2013-2020 Lawrence Livermore National Security, LLC and other
+# Spack Project Developers. See the top-level COPYRIGHT file for details.
+#
+# SPDX-License-Identifier: (Apache-2.0 OR MIT)
+
+# Package automatically generated using 'pip2spack' converter
+
+
+class {{ package_name }}(PythonPackage):
+    """
+    {{ summary }}
+    """
+
+    homepage = "{{ homepage }}"
+    url      = "{{ url }}"
+
+    {% for v in versions|reverse %}
+    version('{{ v[0] }}', sha256='{{ v[1] }}'){% endfor %}
+
+    # depends_on('python@2.7:2.8,3.4:', type=('build', 'run'))
+    {% if depends_on_setuptools %}
+    depends_on('py-setuptools', type='build')
+    {% else %}
+    # depends_on('py-setuptools', type='build')
+    {% endif %}
+
+    def build_args(self, spec, prefix):
+        # FIXME: Add arguments other than --prefix
+        # FIXME: If not needed delete this function
+        args = []
+        return args
```

### Comparing `pip2spack-1.4.1/pip2spack.egg-info/PKG-INFO` & `pip2spack-2.0.0a0/pip2spack.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,105 +1,101 @@
-Metadata-Version: 2.1
-Name: pip2spack
-Version: 1.4.1
-Summary: Automatically create and update a spack package base on the pypi.org information
-Home-page: https://github.com/NexSabre/pip2spack
-Author: Nex Sabre
-Author-email: nexsabre@protonmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pip2Spack
-![Test](https://github.com/NexSabre/pip2spack/workflows/Test/badge.svg?branch=master)
-[![PyPI version](https://badge.fury.io/py/pip2spack.svg)](https://badge.fury.io/py/pip2spack)
-
-Automatically create and update a spack package base on the pypi.org information.
-
-__Cons__:
- - Faster package creation than using the default option `spack create`
- - Automatic updating of existing packages with information contained on pypi.org
- 
- 
-## TL;DR
-```
-// install 
-pip install pip2spack 
-
-// create new one
-pip2spack create jsl
-
-// update a internal (bultin) package
-pip2spack update codecov 
-
-// download latest package locally 
-pip2spack download jsl codecov
-```
-
-
-## Installation
-Later, the package will be added into pypi repository.
-```
-pip install pip2spack
-```
-
-## Build
-To build a .whl package
-
-```
-pip install setuptools wheel twine
-python setup.py sdist bdist_wheel
-```
-
-Than go to `dist` directory and type
-
-```
-pip install pip2spack-1.0-py3-none-any.whl
-```
-
-## Run
-Before you run the script download a spack and export `SPACK_ROOT`. 
-### Create a new package
-To run a script, provide a package names:
-```
-pip2spack create {package_names_for_convert}
-```
-
-Example for creation one new package:
-```
-pip2spack create jsl 
-```
-
-you can also create more than one in single run:
-```
-pip2spack create jsl codecov
-```
-
-### Updating existing packages (builtin)
-Since v0.2, pip2spack is able to update builtin packages to newest version base on the pypi.org information.
-
-__No more adding a new version thru Spack's Pull Requests!__ 
-
-Example:
-```
-pip2spack update codecov
-```
-
-__Notice:__ You can not to create and update packages at once. These operations are separated (in actual version)
-
-
-### Downloading a newest packages locally
-Since v1.1, pip2spack is able to download latest `.tar.gz`/`.whl` package locally, using `download` command
-
-Example:
-```
-pip2spack download jsl codecov
-```
-
-Packages will be stored at the `temp` directory (depends on the OS), proper information wit storage place will be displayed.
-
-
+Metadata-Version: 2.1
+Name: pip2spack
+Version: 2.0.0a0
+Summary: Automatically create and update a spack package base on the pypi.org information
+Home-page: https://github.com/NexSabre/pip2spack
+Author: Nex Sabre
+Author-email: nexsabre@protonmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pip2Spack
+![Test](https://github.com/NexSabre/pip2spack/workflows/Test/badge.svg?branch=master)
+[![PyPI version](https://badge.fury.io/py/pip2spack.svg)](https://badge.fury.io/py/pip2spack)
+
+Automatically create and update a spack package base on the pypi.org information.
+
+__Cons__:
+ - Faster package creation than using the default option `spack create`
+ - Automatic updating of existing packages with information contained on pypi.org
+ 
+ 
+## TL;DR
+```
+// install 
+pip install pip2spack 
+
+// create new one
+pip2spack create jsl
+
+// update a internal (bultin) package
+pip2spack update codecov 
+
+// download latest package locally 
+pip2spack download jsl codecov
+```
+
+
+## Installation
+Later, the package will be added into pypi repository.
+```
+pip install pip2spack
+```
+
+## Build
+To build a .whl package
+
+```
+pip install setuptools wheel twine
+python setup.py sdist bdist_wheel
+```
+
+Than go to `dist` directory and type
+
+```
+pip install pip2spack-1.0-py3-none-any.whl
+```
+
+## Run
+Before you run the script download a spack and export `SPACK_ROOT`. 
+### Create a new package
+To run a script, provide a package names:
+```
+pip2spack create {package_names_for_convert}
+```
+
+Example for creation one new package:
+```
+pip2spack create jsl 
+```
+
+you can also create more than one in single run:
+```
+pip2spack create jsl codecov
+```
+
+### Updating existing packages (builtin)
+Since v0.2, pip2spack is able to update builtin packages to newest version base on the pypi.org information.
+
+__No more adding a new version thru Spack's Pull Requests!__ 
+
+Example:
+```
+pip2spack update codecov
+```
+
+__Notice:__ You can not to create and update packages at once. These operations are separated (in actual version)
+
+
+### Downloading a newest packages locally
+Since v1.1, pip2spack is able to download latest `.tar.gz`/`.whl` package locally, using `download` command
+
+Example:
+```
+pip2spack download jsl codecov
+```
+
+Packages will be stored at the `temp` directory (depends on the OS), proper information wit storage place will be displayed.
```

### Comparing `pip2spack-1.4.1/pip2spack.egg-info/SOURCES.txt` & `pip2spack-2.0.0a0/pip2spack.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 LICENSE
 README.md
 setup.py
 pip2spack/__init__.py
+pip2spack/__main__.py
 pip2spack.egg-info/PKG-INFO
 pip2spack.egg-info/SOURCES.txt
 pip2spack.egg-info/dependency_links.txt
 pip2spack.egg-info/entry_points.txt
 pip2spack.egg-info/requires.txt
 pip2spack.egg-info/top_level.txt
 pip2spack/actions/__init__.py
-pip2spack/actions/action.py
-pip2spack/actions/action_dispatcher.py
-pip2spack/actions/version.py
 pip2spack/actions/create/__init__.py
 pip2spack/actions/create/create_action.py
 pip2spack/actions/dowload/__init__.py
 pip2spack/actions/dowload/download_action.py
 pip2spack/actions/update/__init__.py
 pip2spack/actions/update/update_action.py
 pip2spack/core/__init__.py
@@ -23,18 +21,15 @@
 pip2spack/core/pypi_package.py
 pip2spack/core/spack_repository.py
 pip2spack/core/verification.py
 pip2spack/framework/__init__.py
 pip2spack/framework/constants.py
 pip2spack/framework/helpers.py
 pip2spack/framework/messages.py
-pip2spack/main/__init__.py
-pip2spack/main/main.py
 pip2spack/templates/__init__.py
 pip2spack/templates/package.j2
 tests/__init__.py
 tests/pip2spack/__init__.py
 tests/pip2spack/core/__init__.py
 tests/pip2spack/core/conftest.py
 tests/pip2spack/core/mocks.py
-tests/pip2spack/core/test_pypi_package.py
-tests/pip2spack/core/test_verification.py
+tests/pip2spack/core/test_pypi_package.py
```

### Comparing `pip2spack-1.4.1/tests/pip2spack/core/conftest.py` & `pip2spack-2.0.0a0/tests/pip2spack/core/conftest.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import pytest
-from pytest_mock import MockFixture
-
-from tests.pip2spack.core.mocks import (
-    PYPI_CONFIGSHELL_FB_RESPONSE_MOCK,
-    PYPI_CTYPESGEN_RESPONSE_MOCK,
-    PYPI_RESPONSES,
-)
-
-
-@pytest.fixture
-def mock_pypi_configshell_fb_response(mocker: MockFixture) -> None:
-    mocker.patch(
-        "pip2spack.core.pypi_package.PyPiPackage._download_missing_information",
-        return_value=PYPI_CONFIGSHELL_FB_RESPONSE_MOCK,
-    )
-
-
-@pytest.fixture
-def mock_pypi_jsl_response(mocker: MockFixture) -> None:
-    mocker.patch(
-        "pip2spack.core.pypi_package.PyPiPackage._download_missing_information",
-        return_value=PYPI_RESPONSES["jsl"],
-    )
-
-
-@pytest.fixture
-def mock_pypi_ctypesgen_response(mocker: MockFixture) -> None:
-    mocker.patch(
-        "pip2spack.core.pypi_package.PyPiPackage._download_missing_information",
-        return_value=PYPI_CTYPESGEN_RESPONSE_MOCK["ctypesgen"],
-    )
+import pytest
+from pytest_mock import MockFixture
+
+from tests.pip2spack.core.mocks import (
+    PYPI_CONFIGSHELL_FB_RESPONSE_MOCK,
+    PYPI_CTYPESGEN_RESPONSE_MOCK,
+    PYPI_RESPONSES,
+)
+
+
+@pytest.fixture
+def mock_pypi_configshell_fb_response(mocker: MockFixture) -> None:
+    mocker.patch(
+        "pip2spack.core.pypi_package.PyPiPackage._download_missing_information",
+        return_value=PYPI_CONFIGSHELL_FB_RESPONSE_MOCK,
+    )
+
+
+@pytest.fixture
+def mock_pypi_jsl_response(mocker: MockFixture) -> None:
+    mocker.patch(
+        "pip2spack.core.pypi_package.PyPiPackage._download_missing_information",
+        return_value=PYPI_RESPONSES["jsl"],
+    )
+
+
+@pytest.fixture
+def mock_pypi_ctypesgen_response(mocker: MockFixture) -> None:
+    mocker.patch(
+        "pip2spack.core.pypi_package.PyPiPackage._download_missing_information",
+        return_value=PYPI_CTYPESGEN_RESPONSE_MOCK["ctypesgen"],
+    )
```

### Comparing `pip2spack-1.4.1/tests/pip2spack/core/test_pypi_package.py` & `pip2spack-2.0.0a0/tests/pip2spack/core/test_pypi_package.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from pip2spack.core.pypi_package import PyPiPackage
-
-
-class TestPyPiPackage:
-    def test_pypi_package__generate_correct_path_for_package_with_dash_in_name(
-        self, mock_pypi_configshell_fb_response: None
-    ) -> None:
-        """Base on the issue #16 https://github.com/NexSabre/pip2spack/issues/16"""
-        assert (
-            PyPiPackage("configshell-fb").url
-            == "https://pypi.io/packages/source/c/configshell-fb/configshell-fb-1.1.29.tar.gz"
-        )
-
-    def test_pypi_package__verify_package_name_builder__configshell_fb(
-        self, mock_pypi_configshell_fb_response: None
-    ):
-        assert PyPiPackage("configshell-fb").package_name_builder() == "PyConfigshellFb"
-
-    def test_pypi_package__verify_package_name_builder__jsl(
-        self, mock_pypi_jsl_response: None
-    ) -> None:
-        assert PyPiPackage("jsl").package_name_builder() == "PyJsl"
-
-    def test_pypi_package__package_name_builder_should_replace_dash_in_the_info_name(
-        self, mock_pypi_jsl_response: None
-    ) -> None:
-        package = PyPiPackage("jsl")
-        package.content["info"]["name"] = "jsl-up"
-
-        assert package.package_name_builder() == "PyJslUp"
-
-    def test_pypi_package__test_generate_data_return_message(
-        self, mock_pypi_jsl_response: None
-    ) -> None:
-        return_message = PyPiPackage("jsl")._generate_data()
-        for k, v in return_message.items():
-            if k == "depends_on_setuptools":
-                continue
-            assert v, "Should be True"
-
-    def test_pypi_package__ctypesgen_should_be_categorized_as_not_source(
-        self, mock_pypi_ctypesgen_response: None
-    ) -> None:
-        assert not PyPiPackage(
-            "ctypesgen"
-        ).source, (
-            "Package should be tread as wheel package, source should be unavailable"
-        )
+from pip2spack.core.pypi_package import PyPiPackage
+
+
+class TestPyPiPackage:
+    def test_pypi_package__generate_correct_path_for_package_with_dash_in_name(
+        self, mock_pypi_configshell_fb_response: None
+    ) -> None:
+        """Base on the issue #16 https://github.com/NexSabre/pip2spack/issues/16"""
+        assert (
+            PyPiPackage("configshell-fb").url
+            == "https://pypi.io/packages/source/c/configshell-fb/configshell-fb-1.1.29.tar.gz"
+        )
+
+    def test_pypi_package__verify_package_name_builder__configshell_fb(
+        self, mock_pypi_configshell_fb_response: None
+    ):
+        assert PyPiPackage("configshell-fb").package_name_builder() == "PyConfigshellFb"
+
+    def test_pypi_package__verify_package_name_builder__jsl(
+        self, mock_pypi_jsl_response: None
+    ) -> None:
+        assert PyPiPackage("jsl").package_name_builder() == "PyJsl"
+
+    def test_pypi_package__package_name_builder_should_replace_dash_in_the_info_name(
+        self, mock_pypi_jsl_response: None
+    ) -> None:
+        package = PyPiPackage("jsl")
+        package.content["info"]["name"] = "jsl-up"
+
+        assert package.package_name_builder() == "PyJslUp"
+
+    def test_pypi_package__test_generate_data_return_message(
+        self, mock_pypi_jsl_response: None
+    ) -> None:
+        return_message = PyPiPackage("jsl")._generate_data()
+        for k, v in return_message.items():
+            if k == "depends_on_setuptools":
+                continue
+            assert v, "Should be True"
+
+    def test_pypi_package__ctypesgen_should_be_categorized_as_not_source(
+        self, mock_pypi_ctypesgen_response: None
+    ) -> None:
+        assert not PyPiPackage(
+            "ctypesgen"
+        ).source, (
+            "Package should be tread as wheel package, source should be unavailable"
+        )
```

