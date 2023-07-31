# Comparing `tmp/pyKVFinder-0.6.2.tar.gz` & `tmp/pyKVFinder-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyKVFinder-0.6.2.tar", last modified: Tue Jun 27 14:28:19 2023, max compression
+gzip compressed data, was "pyKVFinder-0.6.3.tar", last modified: Mon Jul 31 16:28:17 2023, max compression
```

## Comparing `pyKVFinder-0.6.2.tar` & `pyKVFinder-0.6.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:28:19.473276 pyKVFinder-0.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:28:19.469276 pyKVFinder-0.6.2/C/
--rw-r--r--   0 runner    (1001) docker     (123)   104503 2023-06-27 14:28:05.000000 pyKVFinder-0.6.2/C/numpy.i
--rw-r--r--   0 runner    (1001) docker     (123)    78654 2023-06-27 14:28:05.000000 pyKVFinder-0.6.2/C/pyKVFinder.c
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-06-27 14:28:05.000000 pyKVFinder-0.6.2/C/pyKVFinder.h
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-06-27 14:28:05.000000 pyKVFinder-0.6.2/C/pyKVFinder.i
--rw-r--r--   0 runner    (1001) docker     (123)    35140 2023-06-27 14:28:05.000000 pyKVFinder-0.6.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-27 14:28:05.000000 pyKVFinder-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    44581 2023-06-27 14:28:19.473276 pyKVFinder-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-06-27 14:28:05.000000 pyKVFinder-0.6.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:28:19.469276 pyKVFinder-0.6.2/pyKVFinder/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:28:19.473276 pyKVFinder-0.6.2/pyKVFinder/data/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/EisenbergWeiss.toml
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/HessaHeijne.toml
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/KyteDoolittle.toml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/MoonFleming.toml
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/RadzickaWolfenden.toml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/WimleyWhite.toml
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/ZhaoLondon.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:28:19.473276 pyKVFinder-0.6.2/pyKVFinder/data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   338350 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb
--rw-r--r--   0 runner    (1001) docker     (123)   226706 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/tests/1FMO.pdb
--rw-r--r--   0 runner    (1001) docker     (123)    88538 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/tests/1FMO.xyz
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/tests/ADN.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/tests/ADN.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/tests/ClO4.pdb
--rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/tests/PKI.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/tests/custom-box.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/tests/residues-box.toml
--rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/data/vdw.dat
--rw-r--r--   0 runner    (1001) docker     (123)   107710 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    71046 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    63360 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyKVFinder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 14:28:19.469276 pyKVFinder-0.6.2/pyKVFinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44581 2023-06-27 14:28:19.000000 pyKVFinder-0.6.2/pyKVFinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-27 14:28:19.000000 pyKVFinder-0.6.2/pyKVFinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 14:28:19.000000 pyKVFinder-0.6.2/pyKVFinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-27 14:28:19.000000 pyKVFinder-0.6.2/pyKVFinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-27 14:28:19.000000 pyKVFinder-0.6.2/pyKVFinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-27 14:28:19.000000 pyKVFinder-0.6.2/pyKVFinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 14:28:19.473276 pyKVFinder-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-27 14:28:06.000000 pyKVFinder-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:28:17.393382 pyKVFinder-0.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:28:17.389382 pyKVFinder-0.6.3/C/
+-rw-r--r--   0 runner    (1001) docker     (123)   104503 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/C/numpy.i
+-rw-r--r--   0 runner    (1001) docker     (123)    78654 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/C/pyKVFinder.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/C/pyKVFinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/C/pyKVFinder.i
+-rw-r--r--   0 runner    (1001) docker     (123)    35140 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    44581 2023-07-31 16:28:17.393382 pyKVFinder-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:28:17.389382 pyKVFinder-0.6.3/pyKVFinder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/pyKVFinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/pyKVFinder/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:28:17.389382 pyKVFinder-0.6.3/pyKVFinder/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/pyKVFinder/data/EisenbergWeiss.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/pyKVFinder/data/HessaHeijne.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/pyKVFinder/data/KyteDoolittle.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/pyKVFinder/data/MoonFleming.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/pyKVFinder/data/RadzickaWolfenden.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/pyKVFinder/data/WimleyWhite.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/pyKVFinder/data/ZhaoLondon.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:28:17.393382 pyKVFinder-0.6.3/pyKVFinder/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   338350 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)   226706 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/pyKVFinder/data/tests/1FMO.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)    88538 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/pyKVFinder/data/tests/1FMO.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/pyKVFinder/data/tests/ADN.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/pyKVFinder/data/tests/ADN.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/pyKVFinder/data/tests/ClO4.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/pyKVFinder/data/tests/PKI.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/pyKVFinder/data/tests/custom-box.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/pyKVFinder/data/tests/residues-box.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/pyKVFinder/data/vdw.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   107710 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/pyKVFinder/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71046 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/pyKVFinder/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63360 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/pyKVFinder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:28:17.389382 pyKVFinder-0.6.3/pyKVFinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44581 2023-07-31 16:28:17.000000 pyKVFinder-0.6.3/pyKVFinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-31 16:28:17.000000 pyKVFinder-0.6.3/pyKVFinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 16:28:17.000000 pyKVFinder-0.6.3/pyKVFinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-31 16:28:17.000000 pyKVFinder-0.6.3/pyKVFinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-31 16:28:17.000000 pyKVFinder-0.6.3/pyKVFinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 16:28:17.000000 pyKVFinder-0.6.3/pyKVFinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 16:28:17.393382 pyKVFinder-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-31 16:28:05.000000 pyKVFinder-0.6.3/setup.py
```

### Comparing `pyKVFinder-0.6.2/C/numpy.i` & `pyKVFinder-0.6.3/C/numpy.i`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.2/C/pyKVFinder.c` & `pyKVFinder-0.6.3/C/pyKVFinder.c`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.2/C/pyKVFinder.h` & `pyKVFinder-0.6.3/C/pyKVFinder.h`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.2/C/pyKVFinder.i` & `pyKVFinder-0.6.3/C/pyKVFinder.i`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.2/LICENSE.txt` & `pyKVFinder-0.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.2/PKG-INFO` & `pyKVFinder-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyKVFinder
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python package to detect and characterize cavities in biomolecular structures
 Author: Helder Veras Ribeiro Filho, Luiz Fernando Giolo Alves, Gabriel Ernesto Jara, Leandro Oliveira Bortot, José Geraldo de Carvalho Pereira, Paulo Sergio Lopes-de-Oliveira
 Author-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 Maintainer-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `pyKVFinder-0.6.2/README.rst` & `pyKVFinder-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.2/pyKVFinder/__init__.py` & `pyKVFinder-0.6.3/pyKVFinder/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,13 +27,13 @@
 --------
 * GitHub repository: https://github.com/LBC-LNBio/pyKVFinder
 
 * Documentation: https://lbc-lnbio.github.io/pyKVFinder
 """
 
 __name__ = "pyKVFinder"
-__version__ = "0.6.2"
+__version__ = "0.6.3"
 license = "GNU GPL-3.0 License"
 
 from .utils import *
 from .grid import *
 from .main import *
```

### Comparing `pyKVFinder-0.6.2/pyKVFinder/argparser.py` & `pyKVFinder-0.6.3/pyKVFinder/argparser.py`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.2/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb` & `pyKVFinder-0.6.3/pyKVFinder/data/tests/1FMO.KVFinder.output.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.2/pyKVFinder/data/tests/1FMO.pdb` & `pyKVFinder-0.6.3/pyKVFinder/data/tests/1FMO.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.2/pyKVFinder/data/tests/1FMO.xyz` & `pyKVFinder-0.6.3/pyKVFinder/data/tests/1FMO.xyz`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.2/pyKVFinder/data/tests/ADN.pdb` & `pyKVFinder-0.6.3/pyKVFinder/data/tests/ADN.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.2/pyKVFinder/data/tests/ADN.xyz` & `pyKVFinder-0.6.3/pyKVFinder/data/tests/ADN.xyz`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.2/pyKVFinder/data/tests/PKI.pdb` & `pyKVFinder-0.6.3/pyKVFinder/data/tests/PKI.pdb`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.2/pyKVFinder/data/vdw.dat` & `pyKVFinder-0.6.3/pyKVFinder/data/vdw.dat`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.2/pyKVFinder/grid.py` & `pyKVFinder-0.6.3/pyKVFinder/grid.py`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.2/pyKVFinder/main.py` & `pyKVFinder-0.6.3/pyKVFinder/main.py`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.2/pyKVFinder/utils.py` & `pyKVFinder-0.6.3/pyKVFinder/utils.py`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.2/pyKVFinder.egg-info/PKG-INFO` & `pyKVFinder-0.6.3/pyKVFinder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyKVFinder
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python package to detect and characterize cavities in biomolecular structures
 Author: Helder Veras Ribeiro Filho, Luiz Fernando Giolo Alves, Gabriel Ernesto Jara, Leandro Oliveira Bortot, José Geraldo de Carvalho Pereira, Paulo Sergio Lopes-de-Oliveira
 Author-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 Maintainer-email: João Victor da Silva Guerra <jvsguerra@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `pyKVFinder-0.6.2/pyKVFinder.egg-info/SOURCES.txt` & `pyKVFinder-0.6.3/pyKVFinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyKVFinder-0.6.2/pyproject.toml` & `pyKVFinder-0.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -42,22 +42,22 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
     "toml==0.10.2",
-    "numpy==1.25.0",
-    "matplotlib==3.7.1",
+    "numpy==1.25.1",
+    "matplotlib==3.7.2",
     "plotly==5.15.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-dev = ["pytest==7.4.0", "pytest-cov==4.1.0", "black==23.3.0", "flake8==6.0.0"]
+dev = ["pytest==7.4.0", "pytest-cov==4.1.0", "black==23.7.0", "flake8==6.1.0"]
 
 [project.urls]
 homepage = "https://github.com/LBC-LNBio/pyKVFinder/"
 documentation = "https://lbc-lnbio.github.io/pyKVFinder/"
 issues = "https://github.com/LBC-LNBio/pyKVFinder/issues"
 
 [project.scripts]
```

### Comparing `pyKVFinder-0.6.2/setup.py` & `pyKVFinder-0.6.3/setup.py`

 * *Files identical despite different names*

