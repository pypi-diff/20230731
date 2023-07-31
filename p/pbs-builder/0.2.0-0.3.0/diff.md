# Comparing `tmp/pbs_builder-0.2.0.tar.gz` & `tmp/pbs_builder-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbs_builder-0.2.0.tar", max compression
+gzip compressed data, was "pbs_builder-0.3.0.tar", max compression
```

## Comparing `pbs_builder-0.2.0.tar` & `pbs_builder-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1070 2023-06-30 08:59:19.000000 pbs_builder-0.2.0/LICENSE
--rw-r--r--   0        0        0     8893 2023-07-19 01:58:06.000000 pbs_builder-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-07-19 01:28:55.000934 pbs_builder-0.2.0/pbs_builder/__init__.py
--rwxr-xr-x   0        0        0    36544 2023-07-19 01:41:40.000000 pbs_builder-0.2.0/pbs_builder/qbatch.py
--rwxr-xr-x   0        0        0      695 2023-07-19 01:50:51.000000 pbs_builder-0.2.0/pbs_builder/qcancel.py
--rw-r--r--   0        0        0      667 2023-07-19 01:58:31.000000 pbs_builder-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     9645 1970-01-01 00:00:00.000000 pbs_builder-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-19 02:02:11.000000 pbs_builder-0.3.0/LICENSE
+-rw-r--r--   0        0        0      697 2023-07-31 08:58:00.000000 pbs_builder-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-19 02:03:05.000000 pbs_builder-0.3.0/pbs_builder/__init__.py
+-rwxr-xr-x   0        0        0    22740 2023-07-31 09:48:03.000000 pbs_builder-0.3.0/pbs_builder/bin/pestat
+-rwxr-xr-x   0        0        0      203 2023-07-31 09:44:00.000000 pbs_builder-0.3.0/pbs_builder/pestat.py
+-rwxr-xr-x   0        0        0    36544 2023-07-19 02:02:11.000000 pbs_builder-0.3.0/pbs_builder/qbatch.py
+-rwxr-xr-x   0        0        0      695 2023-07-19 02:02:11.000000 pbs_builder-0.3.0/pbs_builder/qcancel.py
+-rw-r--r--   0        0        0      738 2023-07-31 09:45:05.000000 pbs_builder-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 pbs_builder-0.3.0/PKG-INFO
```

### Comparing `pbs_builder-0.2.0/LICENSE` & `pbs_builder-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pbs_builder-0.2.0/pbs_builder/qbatch.py` & `pbs_builder-0.3.0/pbs_builder/qbatch.py`

 * *Files identical despite different names*

### Comparing `pbs_builder-0.2.0/pbs_builder/qcancel.py` & `pbs_builder-0.3.0/pbs_builder/qcancel.py`

 * *Files identical despite different names*

### Comparing `pbs_builder-0.2.0/pyproject.toml` & `pbs_builder-0.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 [tool.poetry]
 name = "pbs-builder"
-version = "0.2.0"
+version = "0.3.0"
 description = "The workflow management system for scalable data analyses."
 authors = ["Jinyang Zhang <zhangjinyang@biols.ac.cn>"]
 readme = "README.md"
 license = "LICENSE"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.7"
 ]
+include = ["pbs_builder/bin/pestat"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 tomli = "^2.0.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.4.0"
 
 [tool.poetry.scripts]
 qbatch = 'pbs_builder.qbatch:run'
 qcancel = 'pbs_builder.qcancel:run'
+pestat = 'pbs_builder.pestat:run'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

