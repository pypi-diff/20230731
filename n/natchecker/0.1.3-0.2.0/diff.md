# Comparing `tmp/natchecker-0.1.3.tar.gz` & `tmp/natchecker-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/natchecker-0.1.3.tar", last modified: Mon Jul 31 06:10:46 2023, max compression
+gzip compressed data, was "dist/natchecker-0.2.0.tar", last modified: Mon Jul 31 08:05:58 2023, max compression
```

## Comparing `natchecker-0.1.3.tar` & `natchecker-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 songe      (501) staff       (20)        0 2023-07-31 06:10:46.885180 natchecker-0.1.3/
--rw-r--r--   0 songe      (501) staff       (20)      414 2023-07-31 06:10:46.883991 natchecker-0.1.3/PKG-INFO
--rw-r--r--   0 songe      (501) staff       (20)       80 2023-07-31 03:44:51.000000 natchecker-0.1.3/README.md
-drwxr-xr-x   0 songe      (501) staff       (20)        0 2023-07-31 06:10:46.872980 natchecker-0.1.3/natchecker.egg-info/
--rw-r--r--   0 songe      (501) staff       (20)      414 2023-07-31 06:10:46.000000 natchecker-0.1.3/natchecker.egg-info/PKG-INFO
--rw-r--r--   0 songe      (501) staff       (20)      252 2023-07-31 06:10:46.000000 natchecker-0.1.3/natchecker.egg-info/SOURCES.txt
--rw-r--r--   0 songe      (501) staff       (20)        1 2023-07-31 06:10:46.000000 natchecker-0.1.3/natchecker.egg-info/dependency_links.txt
--rw-r--r--   0 songe      (501) staff       (20)       46 2023-07-31 06:10:46.000000 natchecker-0.1.3/natchecker.egg-info/entry_points.txt
--rw-r--r--   0 songe      (501) staff       (20)        9 2023-07-31 06:10:46.000000 natchecker-0.1.3/natchecker.egg-info/requires.txt
--rw-r--r--   0 songe      (501) staff       (20)        4 2023-07-31 06:10:46.000000 natchecker-0.1.3/natchecker.egg-info/top_level.txt
--rw-r--r--   0 songe      (501) staff       (20)       38 2023-07-31 06:10:46.886579 natchecker-0.1.3/setup.cfg
--rwxr-xr-x   0 songe      (501) staff       (20)      628 2023-07-31 06:10:39.000000 natchecker-0.1.3/setup.py
-drwxr-xr-x   0 songe      (501) staff       (20)        0 2023-07-31 06:10:46.882921 natchecker-0.1.3/src/
--rw-r--r--   0 songe      (501) staff       (20)        0 2023-07-31 06:10:23.000000 natchecker-0.1.3/src/__init__.py
--rw-r--r--   0 songe      (501) staff       (20)    36794 2023-07-31 03:38:35.000000 natchecker-0.1.3/src/main.py
+drwxr-xr-x   0 songe      (501) staff       (20)        0 2023-07-31 08:05:58.077510 natchecker-0.2.0/
+-rw-r--r--   0 songe      (501) staff       (20)       33 2023-07-31 06:11:33.000000 natchecker-0.2.0/.gitignore
+-rw-r--r--   0 songe      (501) staff       (20)      257 2023-07-31 06:13:01.000000 natchecker-0.2.0/Makefile
+-rw-r--r--   0 songe      (501) staff       (20)      489 2023-07-31 08:05:58.076824 natchecker-0.2.0/PKG-INFO
+-rw-r--r--   0 songe      (501) staff       (20)      123 2023-07-31 06:15:32.000000 natchecker-0.2.0/README.md
+drwxr-xr-x   0 songe      (501) staff       (20)        0 2023-07-31 08:05:58.058210 natchecker-0.2.0/natchecker.egg-info/
+-rw-r--r--   0 songe      (501) staff       (20)      489 2023-07-31 08:05:57.000000 natchecker-0.2.0/natchecker.egg-info/PKG-INFO
+-rw-r--r--   0 songe      (501) staff       (20)      272 2023-07-31 08:05:57.000000 natchecker-0.2.0/natchecker.egg-info/SOURCES.txt
+-rw-r--r--   0 songe      (501) staff       (20)        1 2023-07-31 08:05:57.000000 natchecker-0.2.0/natchecker.egg-info/dependency_links.txt
+-rw-r--r--   0 songe      (501) staff       (20)       46 2023-07-31 08:05:57.000000 natchecker-0.2.0/natchecker.egg-info/entry_points.txt
+-rw-r--r--   0 songe      (501) staff       (20)       29 2023-07-31 08:05:57.000000 natchecker-0.2.0/natchecker.egg-info/requires.txt
+-rw-r--r--   0 songe      (501) staff       (20)        4 2023-07-31 08:05:57.000000 natchecker-0.2.0/natchecker.egg-info/top_level.txt
+-rw-r--r--   0 songe      (501) staff       (20)       38 2023-07-31 08:05:58.078861 natchecker-0.2.0/setup.cfg
+-rwxr-xr-x   0 songe      (501) staff       (20)      654 2023-07-31 07:19:40.000000 natchecker-0.2.0/setup.py
+drwxr-xr-x   0 songe      (501) staff       (20)        0 2023-07-31 08:05:58.062155 natchecker-0.2.0/src/
+-rw-r--r--   0 songe      (501) staff       (20)        0 2023-07-31 06:10:23.000000 natchecker-0.2.0/src/__init__.py
+-rw-r--r--   0 songe      (501) staff       (20)    19702 2023-07-31 08:03:51.000000 natchecker-0.2.0/src/main.py
```

### Comparing `natchecker-0.1.3/setup.py` & `natchecker-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='natchecker',
-    version='0.1.3',
+    version='0.2.0',
     author='onewesong',
     author_email='onewesong@gmail.com',
     url='https://github.com/onewesong/natchecker',
     description='check nat type by stun server.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
-    install_requires=['argparse'],
+    install_requires=['argparse', 'ipaddress', 'netifaces'],
     entry_points={'console_scripts': [
         'natchecker=src.main:main',
     ]},
 )
```

