# Comparing `tmp/maci-0.5.1.tar.gz` & `tmp/maci-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maci-0.5.1.tar", last modified: Sun Jul 30 03:28:50 2023, max compression
+gzip compressed data, was "maci-0.5.2.tar", last modified: Sun Jul 30 23:20:55 2023, max compression
```

## Comparing `maci-0.5.1.tar` & `maci-0.5.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.846597 maci-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-07-30 03:28:38.000000 maci-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-07-30 03:28:50.846597 maci-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-07-30 03:28:50.000000 maci-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.842597 maci-0.5.1/maci/
--rw-r--r--   0 runner    (1001) docker     (122)     3371 2023-07-30 03:28:50.000000 maci-0.5.1/maci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22867 2023-07-30 03:28:50.000000 maci-0.5.1/maci/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.842597 maci-0.5.1/maci/_hash/
--rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_hash/comparefilehash.py
--rw-r--r--   0 runner    (1001) docker     (122)     3868 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_hash/createfilehash.py
--rw-r--r--   0 runner    (1001) docker     (122)     3454 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_hash/createhash.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.842597 maci-0.5.1/maci/_ini/
--rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_ini/inibuildauto.py
--rw-r--r--   0 runner    (1001) docker     (122)      902 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_ini/inibuildmanual.py
--rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_ini/inidump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_ini/iniload.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.846597 maci-0.5.1/maci/_json/
--rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_json/jsondump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_json/jsondumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_json/jsonload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1236 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_json/jsonloadstr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.846597 maci-0.5.1/maci/_native/
--rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_native/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     2272 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_native/cleanformat.py
--rw-r--r--   0 runner    (1001) docker     (122)     6878 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_native/dump.py
--rw-r--r--   0 runner    (1001) docker     (122)     4376 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_native/dumpraw.py
--rw-r--r--   0 runner    (1001) docker     (122)     6174 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_native/dumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_native/load.py
--rw-r--r--   0 runner    (1001) docker     (122)     2815 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_native/loadattrs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4126 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_native/loaddict.py
--rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_native/loadraw.py
--rw-r--r--   0 runner    (1001) docker     (122)     2591 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_native/loadstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     3502 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_native/loadstrdict.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.846597 maci-0.5.1/maci/_toml/
--rw-r--r--   0 runner    (1001) docker     (122)     2160 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_toml/tomldump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_toml/tomldumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_toml/tomlload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_toml/tomlloadstr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.846597 maci-0.5.1/maci/_xml/
--rw-r--r--   0 runner    (1001) docker     (122)      888 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_xml/xmlbuildmanual.py
--rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_xml/xmldump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1466 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_xml/xmldumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     2015 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_xml/xmlload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_xml/xmlloadstr.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.846597 maci-0.5.1/maci/_yaml/
--rw-r--r--   0 runner    (1001) docker     (122)     2107 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_yaml/yamldump.py
--rw-r--r--   0 runner    (1001) docker     (122)     1124 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_yaml/yamldumpstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_yaml/yamlload.py
--rw-r--r--   0 runner    (1001) docker     (122)     1277 2023-07-30 03:28:50.000000 maci-0.5.1/maci/_yaml/yamlloadstr.py
--rw-r--r--   0 runner    (1001) docker     (122)    75585 2023-07-30 03:28:50.000000 maci-0.5.1/maci/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     7977 2023-07-30 03:28:50.000000 maci-0.5.1/maci/data.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-07-30 03:28:50.000000 maci-0.5.1/maci/error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.842597 maci-0.5.1/maci/ext/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.846597 maci-0.5.1/maci/ext/defusedxml/
--rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-07-30 03:28:50.000000 maci-0.5.1/maci/ext/defusedxml/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-07-30 03:28:50.000000 maci-0.5.1/maci/hint.py
--rw-r--r--   0 runner    (1001) docker     (122)      880 2023-07-30 03:28:50.000000 maci-0.5.1/maci/hint.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.000000 maci-0.5.1/maci/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 03:28:50.842597 maci-0.5.1/maci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-07-30 03:28:50.000000 maci-0.5.1/maci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1199 2023-07-30 03:28:50.000000 maci-0.5.1/maci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-30 03:28:50.000000 maci-0.5.1/maci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-30 03:28:50.000000 maci-0.5.1/maci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-30 03:28:50.000000 maci-0.5.1/maci.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-07-30 03:28:50.846597 maci-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-07-30 03:28:38.000000 maci-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 23:20:55.956621 maci-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-07-30 23:20:45.000000 maci-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-07-30 23:20:55.956621 maci-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-07-30 23:20:55.000000 maci-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 23:20:55.948621 maci-0.5.2/maci/
+-rw-r--r--   0 runner    (1001) docker     (122)     3371 2023-07-30 23:20:55.000000 maci-0.5.2/maci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22867 2023-07-30 23:20:55.000000 maci-0.5.2/maci/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 23:20:55.948621 maci-0.5.2/maci/_hash/
+-rw-r--r--   0 runner    (1001) docker     (122)     2704 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_hash/comparefilehash.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3868 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_hash/createfilehash.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3454 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_hash/createhash.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 23:20:55.952621 maci-0.5.2/maci/_ini/
+-rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_ini/inibuildauto.py
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_ini/inibuildmanual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_ini/inidump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_ini/iniload.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 23:20:55.952621 maci-0.5.2/maci/_json/
+-rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_json/jsondump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_json/jsondumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1685 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_json/jsonload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1236 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_json/jsonloadstr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 23:20:55.952621 maci-0.5.2/maci/_native/
+-rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_native/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2272 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_native/cleanformat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6878 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_native/dump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4376 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_native/dumpraw.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6174 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_native/dumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3615 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_native/load.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2815 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_native/loadattrs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4126 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_native/loaddict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_native/loadraw.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2591 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_native/loadstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3502 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_native/loadstrdict.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 23:20:55.952621 maci-0.5.2/maci/_toml/
+-rw-r--r--   0 runner    (1001) docker     (122)     2160 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_toml/tomldump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_toml/tomldumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_toml/tomlload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_toml/tomlloadstr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 23:20:55.952621 maci-0.5.2/maci/_xml/
+-rw-r--r--   0 runner    (1001) docker     (122)      888 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_xml/xmlbuildmanual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_xml/xmldump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1466 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_xml/xmldumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2015 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_xml/xmlload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1347 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_xml/xmlloadstr.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 23:20:55.952621 maci-0.5.2/maci/_yaml/
+-rw-r--r--   0 runner    (1001) docker     (122)     2107 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_yaml/yamldump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1124 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_yaml/yamldumpstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_yaml/yamlload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1277 2023-07-30 23:20:55.000000 maci-0.5.2/maci/_yaml/yamlloadstr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    76286 2023-07-30 23:20:55.000000 maci-0.5.2/maci/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7977 2023-07-30 23:20:55.000000 maci-0.5.2/maci/data.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-07-30 23:20:55.000000 maci-0.5.2/maci/error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 23:20:55.948621 maci-0.5.2/maci/ext/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 23:20:55.952621 maci-0.5.2/maci/ext/defusedxml/
+-rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-07-30 23:20:55.000000 maci-0.5.2/maci/ext/defusedxml/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-07-30 23:20:55.000000 maci-0.5.2/maci/hint.py
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2023-07-30 23:20:55.000000 maci-0.5.2/maci/hint.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-30 23:20:55.000000 maci-0.5.2/maci/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-30 23:20:55.948621 maci-0.5.2/maci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2494 2023-07-30 23:20:55.000000 maci-0.5.2/maci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1199 2023-07-30 23:20:55.000000 maci-0.5.2/maci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-30 23:20:55.000000 maci-0.5.2/maci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-30 23:20:55.000000 maci-0.5.2/maci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-30 23:20:55.000000 maci-0.5.2/maci.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-07-30 23:20:55.956621 maci-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-07-30 23:20:45.000000 maci-0.5.2/setup.py
```

### Comparing `maci-0.5.1/PKG-INFO` & `maci-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maci
-Version: 0.5.1
+Version: 0.5.2
 Summary: The easy to use library for your data, configuration, and save files
 Author: aaronater10
 Author-email: dev_admin@dunnts.com
 License: MIT
 Project-URL: Docs, https://docs.macilib.org
 Project-URL: Code, https://github.com/aaronater10/maci
 Project-URL: Bugs, https://github.com/aaronater10/maci/issues
@@ -23,15 +23,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # maci
 The easy to use library for your data, configuration, and save files
 
-##### Latest Version: 0.5.1
+##### Latest Version: 0.5.2
 
 #
 
 Import or Export **custom**, or **industry-common**, data, config, and save files easily for your python program or script!
 
 **Use python data types for your data** (literally use python data types as stored values importing them securely vs just importing a .py file) **in any text file**.
```

### Comparing `maci-0.5.1/README.md` & `maci-0.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # maci
 The easy to use library for your data, configuration, and save files
 
-##### Latest Version: 0.5.1
+##### Latest Version: 0.5.2
 
 #
 
 Import or Export **custom**, or **industry-common**, data, config, and save files easily for your python program or script!
 
 **Use python data types for your data** (literally use python data types as stored values importing them securely vs just importing a .py file) **in any text file**.
```

### Comparing `maci-0.5.1/maci/__init__.py` & `maci-0.5.2/maci/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 maci - by aaronater10
 
 A Pythonic Configuration Language & Thin Wrapper Library
 
-Version 0.5.1
+Version 0.5.2
 
 Tutorials and docs: https://docs.macilib.org
 
 Source: https://github.com/aaronater10/maci
 """
-__version__ = '0.5.1'
+__version__ = '0.5.2'
 
 #########################################################################################################
 # Imports
 
 # Exceptions
 from . import error
```

### Comparing `maci-0.5.1/maci/__init__.pyi` & `maci-0.5.2/maci/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # stub file to document public api functions, errors, object types, and doc string comments
 """
 maci - by aaronater10
 
 A Pythonic Configuration Language & Thin Wrapper Library
 
-Version 0.5.1
+Version 0.5.2
 
 Tutorials and docs: https://docs.macilib.org
 
 Source: https://github.com/aaronater10/maci
 """
 #########################################################################################################
 # Imports
```

### Comparing `maci-0.5.1/maci/_hash/comparefilehash.py` & `maci-0.5.2/maci/_hash/comparefilehash.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_hash/createfilehash.py` & `maci-0.5.2/maci/_hash/createfilehash.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_hash/createhash.py` & `maci-0.5.2/maci/_hash/createhash.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_ini/inibuildauto.py` & `maci-0.5.2/maci/_ini/inibuildauto.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_ini/inibuildmanual.py` & `maci-0.5.2/maci/_ini/inibuildmanual.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_ini/inidump.py` & `maci-0.5.2/maci/_ini/inidump.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_ini/iniload.py` & `maci-0.5.2/maci/_ini/iniload.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_json/jsondump.py` & `maci-0.5.2/maci/_json/jsondump.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_json/jsondumpstr.py` & `maci-0.5.2/maci/_json/jsondumpstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_json/jsonload.py` & `maci-0.5.2/maci/_json/jsonload.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_json/jsonloadstr.py` & `maci-0.5.2/maci/_json/jsonloadstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_native/build.py` & `maci-0.5.2/maci/_native/build.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_native/cleanformat.py` & `maci-0.5.2/maci/_native/cleanformat.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_native/dump.py` & `maci-0.5.2/maci/_native/dump.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_native/dumpraw.py` & `maci-0.5.2/maci/_native/dumpraw.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_native/dumpstr.py` & `maci-0.5.2/maci/_native/dumpstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_native/load.py` & `maci-0.5.2/maci/_native/load.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_native/loadattrs.py` & `maci-0.5.2/maci/_native/loadattrs.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_native/loaddict.py` & `maci-0.5.2/maci/_native/loaddict.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_native/loadraw.py` & `maci-0.5.2/maci/_native/loadraw.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_native/loadstr.py` & `maci-0.5.2/maci/_native/loadstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_native/loadstrdict.py` & `maci-0.5.2/maci/_native/loadstrdict.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_toml/tomldump.py` & `maci-0.5.2/maci/_toml/tomldump.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_toml/tomldumpstr.py` & `maci-0.5.2/maci/_toml/tomldumpstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_toml/tomlload.py` & `maci-0.5.2/maci/_toml/tomlload.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_toml/tomlloadstr.py` & `maci-0.5.2/maci/_toml/tomlloadstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_xml/xmlbuildmanual.py` & `maci-0.5.2/maci/_xml/xmlbuildmanual.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_xml/xmldump.py` & `maci-0.5.2/maci/_xml/xmldump.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_xml/xmldumpstr.py` & `maci-0.5.2/maci/_xml/xmldumpstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_xml/xmlload.py` & `maci-0.5.2/maci/_xml/xmlload.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_xml/xmlloadstr.py` & `maci-0.5.2/maci/_xml/xmlloadstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_yaml/yamldump.py` & `maci-0.5.2/maci/_yaml/yamldump.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_yaml/yamldumpstr.py` & `maci-0.5.2/maci/_yaml/yamldumpstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_yaml/yamlload.py` & `maci-0.5.2/maci/_yaml/yamlload.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/_yaml/yamlloadstr.py` & `maci-0.5.2/maci/_yaml/yamlloadstr.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/data.py` & `maci-0.5.2/maci/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1112,15 +1112,14 @@
     """
     Main dump function for file/string dump
     """
     # DUMP STR REQUEST: If this is a str dump request,
     # then set values accordingly
     
     # Error Checks & Collect Error Messages
-    __err_msg_general_error = "Error has occurred and cannot proceed"
     __err_msg_invalid_maciobj = "Invalid maci object passed in. Please use a valid 'MaciDataObj'"
     __err_msg_no_attrs_found = __err_msg_no_attrs_found
 
     if _is_string_request:
         # Set Error Type
         DumpStrError = DumpStr
         # Set Values
@@ -1137,15 +1136,16 @@
 
     # Setup
     __build_data_output: _Any = _StringIO()
     __assignment_glyphs = _Glyphs()
     __skip_object_key = ('_MaciDataObjConstructor', '__maci_obj_format_id')
     __locked_attr_list_key =  '_MaciDataObjConstructor__assignment_locked_attribs'
     __hard_locked_attr_list_key =  '_MaciDataObjConstructor__assignment_hard_locked_attribs'
-    __reference_attr_list_key =  '_MaciDataObjConstructor__assigned_src_reference_attr_map'
+    __src_reference_attr_list_key =  '_MaciDataObjConstructor__assigned_src_reference_attr_map'
+    __dst_reference_attr_list_key =  '_MaciDataObjConstructor__assigned_dst_reference_attr_map'
     __maci_obj_format_id_match = "48448910-fa49-45ca-bd3e-38d7af136af5-7bcece52-e5ee-4272-989d-103f07aa6c0f"
 
     # Set Write Mode: 'a' = append, 'w' = write
     write_mode = 'a' if append else 'w'
 
     # Set Glyph Style to Symbols if Requested - Creates New Object with Same Names
     if use_symbol_glyphs:
@@ -1154,49 +1154,59 @@
             h=__assignment_glyphs.hard_lock,
             l=__assignment_glyphs.lock,
             mh=__assignment_glyphs.ref_hard_lock,
             ml=__assignment_glyphs.ref_lock,
         )
 
     
-    ### MACI Got: Check if MaciDataObj ###
+    ### MACI OBJ: Check if MaciDataObj ###
 
     # Build Out Data
     if (isinstance(data, MaciDataObj)) and (data.__maci_obj_format_id__ == __maci_obj_format_id_match):
-        for key,value in data.__dict__.items():
-            # If Match Prefixes, Skip
+        
+        # Create Reference, Restructure and Shift Parent/Child Key Names to Maintain Relationship Order in Dump Output
+        _maci_data_dict_ref = _deepcopy(data.__dict__)
+
+        # If Found, Move Parent(s) to End of Dict and Maintain Value
+        for parent_name,child_data in data.__dict__[__dst_reference_attr_list_key].items():
+            parent_value = _maci_data_dict_ref.pop(parent_name)
+            _maci_data_dict_ref[parent_name] = parent_value
+            # Move all Children to End of Dict
+            for child_name in child_data:
+                _maci_data_dict_ref.pop(child_name)
+                _maci_data_dict_ref[child_name] = None # does not need original value as it is a reference
+
+        # Build and Set Data
+        for key,value in _maci_data_dict_ref.items():
+            # If Match Skip Prefixes, then Skip
             if not key.startswith(__skip_object_key):
                 # Check Glyph Type and Build Accordingly
 
-                # Reset Values
-                is_set_start_new_line = ''
-                is_set_end_new_line = ''
-
                 # Check for Dunder or Unders
                 _is_dunder_attr = False
                 if key.startswith(f'__'):
                     if (private_attrs or private_dunder_attrs):
                         _is_dunder_attr = True
                     else: continue  # pragma: no cover  # code does work, but py10+ is only passing cov oddly
                 if (key.startswith('_')) and not (_is_dunder_attr):
                     if not (private_attrs or private_under_attrs):
                         continue
                 _is_dunder_attr = False # reset dunder check for single under's
 
                 # Reference Name and Locked
-                if (key in data.__dict__[__reference_attr_list_key]) and (key in data.__dict__[__locked_attr_list_key]):
-                    __build_data_output.write(f'{key} {__assignment_glyphs.ml} {data.__dict__[__reference_attr_list_key][key]}\n')
+                if (key in data.__dict__[__src_reference_attr_list_key]) and (key in data.__dict__[__locked_attr_list_key]):
+                    __build_data_output.write(f'{key} {__assignment_glyphs.ml} {data.__dict__[__src_reference_attr_list_key][key]}\n')
                     continue
                 # Reference Name and Hard Locked
-                if (key in data.__dict__[__reference_attr_list_key]) and (key in data.__dict__[__hard_locked_attr_list_key]):
-                    __build_data_output.write(f'{key} {__assignment_glyphs.mh} {data.__dict__[__reference_attr_list_key][key]}\n')
+                if (key in data.__dict__[__src_reference_attr_list_key]) and (key in data.__dict__[__hard_locked_attr_list_key]):
+                    __build_data_output.write(f'{key} {__assignment_glyphs.mh} {data.__dict__[__src_reference_attr_list_key][key]}\n')
                     continue
                 # Reference Name Only
-                if key in data.__dict__[__reference_attr_list_key]:
-                    __build_data_output.write(f'{key} {__assignment_glyphs.m} {data.__dict__[__reference_attr_list_key][key]}\n')
+                if key in data.__dict__[__src_reference_attr_list_key]:
+                    __build_data_output.write(f'{key} {__assignment_glyphs.m} {data.__dict__[__src_reference_attr_list_key][key]}\n')
                     continue
 
                 # REPR SIGNAL: If certain object type matches, disable repr use
                 repr_signal = __repr_signal(value)
 
                 # Locked Only
                 if key in data.__dict__[__locked_attr_list_key]:
```

### Comparing `maci-0.5.1/maci/data.pyi` & `maci-0.5.2/maci/data.pyi`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/error.py` & `maci-0.5.2/maci/error.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/ext/defusedxml/LICENSE.txt` & `maci-0.5.2/maci/ext/defusedxml/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/hint.py` & `maci-0.5.2/maci/hint.py`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci/hint.pyi` & `maci-0.5.2/maci/hint.pyi`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/maci.egg-info/PKG-INFO` & `maci-0.5.2/maci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maci
-Version: 0.5.1
+Version: 0.5.2
 Summary: The easy to use library for your data, configuration, and save files
 Author: aaronater10
 Author-email: dev_admin@dunnts.com
 License: MIT
 Project-URL: Docs, https://docs.macilib.org
 Project-URL: Code, https://github.com/aaronater10/maci
 Project-URL: Bugs, https://github.com/aaronater10/maci/issues
@@ -23,15 +23,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # maci
 The easy to use library for your data, configuration, and save files
 
-##### Latest Version: 0.5.1
+##### Latest Version: 0.5.2
 
 #
 
 Import or Export **custom**, or **industry-common**, data, config, and save files easily for your python program or script!
 
 **Use python data types for your data** (literally use python data types as stored values importing them securely vs just importing a .py file) **in any text file**.
```

### Comparing `maci-0.5.1/maci.egg-info/SOURCES.txt` & `maci-0.5.2/maci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maci-0.5.1/setup.cfg` & `maci-0.5.2/setup.cfg`

 * *Files identical despite different names*

