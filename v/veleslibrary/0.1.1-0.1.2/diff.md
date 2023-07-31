# Comparing `tmp/veleslibrary-0.1.1.tar.gz` & `tmp/veleslibrary-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veleslibrary-0.1.1.tar", max compression
+gzip compressed data, was "veleslibrary-0.1.2.tar", max compression
```

## Comparing `veleslibrary-0.1.1.tar` & `veleslibrary-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       15 2023-07-02 10:09:22.632265 veleslibrary-0.1.1/README.md
--rw-r--r--   0        0        0      463 2023-07-02 10:09:39.500522 veleslibrary-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-02 10:09:22.632265 veleslibrary-0.1.1/veleslibrary/__init__.py
--rw-r--r--   0        0        0       30 2023-07-02 10:09:22.632265 veleslibrary-0.1.1/veleslibrary/questionnaires/__init__.py
--rw-r--r--   0        0        0       63 2023-07-02 10:09:22.632265 veleslibrary-0.1.1/veleslibrary/questionnaires/pl/__init__.py
--rw-r--r--   0        0        0     3113 2023-07-02 10:09:22.632265 veleslibrary-0.1.1/veleslibrary/questionnaires/pl/questionnaires.py
--rw-r--r--   0        0        0     2289 2023-07-02 10:09:22.632265 veleslibrary-0.1.1/veleslibrary/questionnaires/questionnaires.py
--rw-r--r--   0        0        0       21 2023-07-02 10:09:22.632265 veleslibrary-0.1.1/veleslibrary/tests/__init__.py
--rw-r--r--   0        0        0       44 2023-07-02 10:09:22.632265 veleslibrary-0.1.1/veleslibrary/tests/pl/__init__.py
--rw-r--r--   0        0        0     5161 2023-07-02 10:09:22.632265 veleslibrary-0.1.1/veleslibrary/tests/pl/tests.py
--rw-r--r--   0        0        0     1029 2023-07-02 10:09:22.632265 veleslibrary-0.1.1/veleslibrary/tests/tests.py
--rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 veleslibrary-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       15 2023-07-31 11:03:20.315375 veleslibrary-0.1.2/README.md
+-rw-r--r--   0        0        0      465 2023-07-31 11:03:38.267780 veleslibrary-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-31 11:03:20.319375 veleslibrary-0.1.2/veleslibrary/__init__.py
+-rw-r--r--   0        0        0       30 2023-07-31 11:03:20.319375 veleslibrary-0.1.2/veleslibrary/questionnaires/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-31 11:03:20.319375 veleslibrary-0.1.2/veleslibrary/questionnaires/pl/__init__.py
+-rw-r--r--   0        0        0     3113 2023-07-31 11:03:20.319375 veleslibrary-0.1.2/veleslibrary/questionnaires/pl/questionnaires.py
+-rw-r--r--   0        0        0     2289 2023-07-31 11:03:20.319375 veleslibrary-0.1.2/veleslibrary/questionnaires/questionnaires.py
+-rw-r--r--   0        0        0       21 2023-07-31 11:03:20.319375 veleslibrary-0.1.2/veleslibrary/tests/__init__.py
+-rw-r--r--   0        0        0       44 2023-07-31 11:03:20.319375 veleslibrary-0.1.2/veleslibrary/tests/pl/__init__.py
+-rw-r--r--   0        0        0     5161 2023-07-31 11:03:20.319375 veleslibrary-0.1.2/veleslibrary/tests/pl/tests.py
+-rw-r--r--   0        0        0     1029 2023-07-31 11:03:20.319375 veleslibrary-0.1.2/veleslibrary/tests/tests.py
+-rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 veleslibrary-0.1.2/PKG-INFO
```

### Comparing `veleslibrary-0.1.1/veleslibrary/questionnaires/pl/questionnaires.py` & `veleslibrary-0.1.2/veleslibrary/questionnaires/pl/questionnaires.py`

 * *Files identical despite different names*

### Comparing `veleslibrary-0.1.1/veleslibrary/questionnaires/questionnaires.py` & `veleslibrary-0.1.2/veleslibrary/questionnaires/questionnaires.py`

 * *Files identical despite different names*

### Comparing `veleslibrary-0.1.1/veleslibrary/tests/pl/tests.py` & `veleslibrary-0.1.2/veleslibrary/tests/pl/tests.py`

 * *Files identical despite different names*

### Comparing `veleslibrary-0.1.1/veleslibrary/tests/tests.py` & `veleslibrary-0.1.2/veleslibrary/tests/tests.py`

 * *Files identical despite different names*

