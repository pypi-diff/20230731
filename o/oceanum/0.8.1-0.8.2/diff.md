# Comparing `tmp/oceanum-0.8.1.tar.gz` & `tmp/oceanum-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oceanum-0.8.1.tar", last modified: Sun Jul 30 21:26:15 2023, max compression
+gzip compressed data, was "oceanum-0.8.2.tar", last modified: Mon Jul 31 20:46:33 2023, max compression
```

## Comparing `oceanum-0.8.1.tar` & `oceanum-0.8.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.928190 oceanum-0.8.1/
--rw-rw-r--   0 dave      (1000) dave      (1000)      151 2023-05-14 22:31:40.000000 oceanum-0.8.1/AUTHORS.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     3501 2023-05-14 22:31:40.000000 oceanum-0.8.1/CONTRIBUTING.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1077 2023-05-14 22:31:40.000000 oceanum-0.8.1/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)      262 2023-05-14 22:31:40.000000 oceanum-0.8.1/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)     1089 2023-07-30 21:26:15.928190 oceanum-0.8.1/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      788 2023-05-14 22:31:40.000000 oceanum-0.8.1/README.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.916190 oceanum-0.8.1/docs/
--rw-rw-r--   0 dave      (1000) dave      (1000)      639 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/Makefile
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.912190 oceanum-0.8.1/docs/_build/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.912190 oceanum-0.8.1/docs/_build/html/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.916190 oceanum-0.8.1/docs/_build/html/_static/
--rw-rw-r--   0 dave      (1000) dave      (1000)      286 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/_build/html/_static/file.png
--rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/_build/html/_static/minus.png
--rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/_build/html/_static/plus.png
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.912190 oceanum-0.8.1/docs/_templates/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.916190 oceanum-0.8.1/docs/_templates/autosummary/
--rw-rw-r--   0 dave      (1000) dave      (1000)      481 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/_templates/autosummary/class.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)       73 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/about.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      593 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/api.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.912190 oceanum-0.8.1/docs/classes/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.920190 oceanum-0.8.1/docs/classes/datamesh/
--rw-rw-r--   0 dave      (1000) dave      (1000)      406 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/classes/datamesh/oceanum.datamesh.Catalog.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      713 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/classes/datamesh/oceanum.datamesh.Connector.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      131 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/classes/datamesh/oceanum.datamesh.Datasource.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      116 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/classes/datamesh/oceanum.datamesh.Query.rst
--rwxrwxr-x   0 dave      (1000) dave      (1000)     5654 2023-07-11 03:17:01.000000 oceanum-0.8.1/docs/conf.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      522 2023-07-11 03:17:01.000000 oceanum-0.8.1/docs/index.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1133 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/installation.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      801 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/make.bat
--rw-rw-r--   0 dave      (1000) dave      (1000)       58 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/modules.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      967 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/oceanum.datamesh.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      365 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/oceanum.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1437 2023-05-14 22:31:40.000000 oceanum-0.8.1/docs/usage.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.920190 oceanum-0.8.1/oceanum/
--rw-rw-r--   0 dave      (1000) dave      (1000)      474 2023-07-30 21:26:13.000000 oceanum-0.8.1/oceanum/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      313 2023-05-14 22:31:40.000000 oceanum-0.8.1/oceanum/cli.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.924190 oceanum-0.8.1/oceanum/datamesh/
--rw-rw-r--   0 dave      (1000) dave      (1000)      122 2023-05-14 22:31:40.000000 oceanum-0.8.1/oceanum/datamesh/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3425 2023-05-14 22:31:40.000000 oceanum-0.8.1/oceanum/datamesh/catalog.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    21330 2023-07-30 21:15:42.000000 oceanum-0.8.1/oceanum/datamesh/connection.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    11333 2023-07-30 20:00:11.000000 oceanum-0.8.1/oceanum/datamesh/datasource.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      144 2023-05-14 22:31:40.000000 oceanum-0.8.1/oceanum/datamesh/exceptions.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     7849 2023-07-30 20:00:11.000000 oceanum-0.8.1/oceanum/datamesh/query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     5037 2023-06-14 04:46:09.000000 oceanum-0.8.1/oceanum/datamesh/zarr.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.920190 oceanum-0.8.1/oceanum.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1089 2023-07-30 21:26:15.000000 oceanum-0.8.1/oceanum.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     1372 2023-07-30 21:26:15.000000 oceanum-0.8.1/oceanum.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-07-30 21:26:15.000000 oceanum-0.8.1/oceanum.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       45 2023-07-30 21:26:15.000000 oceanum-0.8.1/oceanum.egg-info/entry_points.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-07-30 21:26:15.000000 oceanum-0.8.1/oceanum.egg-info/not-zip-safe
--rw-rw-r--   0 dave      (1000) dave      (1000)      133 2023-07-30 21:26:15.000000 oceanum-0.8.1/oceanum.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        8 2023-07-30 21:26:15.000000 oceanum-0.8.1/oceanum.egg-info/top_level.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      419 2023-07-30 21:26:15.932190 oceanum-0.8.1/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)     1282 2023-07-30 21:04:55.000000 oceanum-0.8.1/setup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.924190 oceanum-0.8.1/tests/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-14 22:31:40.000000 oceanum-0.8.1/tests/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-30 21:26:15.928190 oceanum-0.8.1/tests/data/
--rw-rw-r--   0 dave      (1000) dave      (1000)    21010 2023-05-14 22:31:40.000000 oceanum-0.8.1/tests/data/grid_data_1.nc
--rw-rw-r--   0 dave      (1000) dave      (1000)  2029589 2023-05-14 22:31:40.000000 oceanum-0.8.1/tests/data/ocean_test_1.mp4
--rw-rw-r--   0 dave      (1000) dave      (1000)     1727 2023-05-14 22:31:40.000000 oceanum-0.8.1/tests/data/point_data_1.csv
--rw-rw-r--   0 dave      (1000) dave      (1000)     1222 2023-05-14 22:31:40.000000 oceanum-0.8.1/tests/test_catalog.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1072 2023-05-14 22:31:40.000000 oceanum-0.8.1/tests/test_datamesh_connect.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1643 2023-05-14 22:31:40.000000 oceanum-0.8.1/tests/test_datamesh_load.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2578 2023-05-14 22:31:40.000000 oceanum-0.8.1/tests/test_datamesh_query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3255 2023-05-14 22:31:40.000000 oceanum-0.8.1/tests/test_datamesh_write.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2958 2023-07-11 22:58:57.000000 oceanum-0.8.1/tests/test_datasource.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1482 2023-07-11 23:07:04.000000 oceanum-0.8.1/tests/test_query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      805 2023-05-14 22:31:40.000000 oceanum-0.8.1/tests/test_video_compat.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:46:33.032474 oceanum-0.8.2/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      151 2023-05-14 22:31:40.000000 oceanum-0.8.2/AUTHORS.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3501 2023-05-14 22:31:40.000000 oceanum-0.8.2/CONTRIBUTING.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1077 2023-05-14 22:31:40.000000 oceanum-0.8.2/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)      262 2023-05-14 22:31:40.000000 oceanum-0.8.2/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1089 2023-07-31 20:46:33.032474 oceanum-0.8.2/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      788 2023-05-14 22:31:40.000000 oceanum-0.8.2/README.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:46:33.016474 oceanum-0.8.2/docs/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      639 2023-05-14 22:31:40.000000 oceanum-0.8.2/docs/Makefile
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:46:32.992474 oceanum-0.8.2/docs/_build/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:46:32.992474 oceanum-0.8.2/docs/_build/html/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:46:33.020474 oceanum-0.8.2/docs/_build/html/_static/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      286 2023-05-14 22:31:40.000000 oceanum-0.8.2/docs/_build/html/_static/file.png
+-rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.8.2/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.8.2/docs/_build/html/_static/plus.png
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:46:32.992474 oceanum-0.8.2/docs/_templates/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:46:33.020474 oceanum-0.8.2/docs/_templates/autosummary/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      481 2023-05-14 22:31:40.000000 oceanum-0.8.2/docs/_templates/autosummary/class.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)       73 2023-05-14 22:31:40.000000 oceanum-0.8.2/docs/about.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      593 2023-05-14 22:31:40.000000 oceanum-0.8.2/docs/api.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:46:32.992474 oceanum-0.8.2/docs/classes/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:46:33.020474 oceanum-0.8.2/docs/classes/datamesh/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      406 2023-05-14 22:31:40.000000 oceanum-0.8.2/docs/classes/datamesh/oceanum.datamesh.Catalog.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      713 2023-05-14 22:31:40.000000 oceanum-0.8.2/docs/classes/datamesh/oceanum.datamesh.Connector.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      131 2023-05-14 22:31:40.000000 oceanum-0.8.2/docs/classes/datamesh/oceanum.datamesh.Datasource.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      116 2023-05-14 22:31:40.000000 oceanum-0.8.2/docs/classes/datamesh/oceanum.datamesh.Query.rst
+-rwxrwxr-x   0 dave      (1000) dave      (1000)     5654 2023-07-11 03:17:01.000000 oceanum-0.8.2/docs/conf.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      522 2023-07-11 03:17:01.000000 oceanum-0.8.2/docs/index.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1133 2023-05-14 22:31:40.000000 oceanum-0.8.2/docs/installation.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      801 2023-05-14 22:31:40.000000 oceanum-0.8.2/docs/make.bat
+-rw-rw-r--   0 dave      (1000) dave      (1000)       58 2023-05-14 22:31:40.000000 oceanum-0.8.2/docs/modules.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      967 2023-05-14 22:31:40.000000 oceanum-0.8.2/docs/oceanum.datamesh.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      365 2023-05-14 22:31:40.000000 oceanum-0.8.2/docs/oceanum.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1437 2023-05-14 22:31:40.000000 oceanum-0.8.2/docs/usage.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:46:33.020474 oceanum-0.8.2/oceanum/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      656 2023-07-31 20:45:10.000000 oceanum-0.8.2/oceanum/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      313 2023-05-14 22:31:40.000000 oceanum-0.8.2/oceanum/cli.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:46:33.024474 oceanum-0.8.2/oceanum/datamesh/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      122 2023-05-14 22:31:40.000000 oceanum-0.8.2/oceanum/datamesh/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3425 2023-05-14 22:31:40.000000 oceanum-0.8.2/oceanum/datamesh/catalog.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    21330 2023-07-30 21:15:42.000000 oceanum-0.8.2/oceanum/datamesh/connection.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    11333 2023-07-30 20:00:11.000000 oceanum-0.8.2/oceanum/datamesh/datasource.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      186 2023-07-31 20:33:46.000000 oceanum-0.8.2/oceanum/datamesh/exceptions.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7849 2023-07-30 20:00:11.000000 oceanum-0.8.2/oceanum/datamesh/query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     5037 2023-06-14 04:46:09.000000 oceanum-0.8.2/oceanum/datamesh/zarr.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:46:33.024474 oceanum-0.8.2/oceanum.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1089 2023-07-31 20:46:32.000000 oceanum-0.8.2/oceanum.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1372 2023-07-31 20:46:32.000000 oceanum-0.8.2/oceanum.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-07-31 20:46:32.000000 oceanum-0.8.2/oceanum.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       45 2023-07-31 20:46:32.000000 oceanum-0.8.2/oceanum.egg-info/entry_points.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-07-31 20:46:32.000000 oceanum-0.8.2/oceanum.egg-info/not-zip-safe
+-rw-rw-r--   0 dave      (1000) dave      (1000)      133 2023-07-31 20:46:32.000000 oceanum-0.8.2/oceanum.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        8 2023-07-31 20:46:32.000000 oceanum-0.8.2/oceanum.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      419 2023-07-31 20:46:33.036474 oceanum-0.8.2/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1282 2023-07-30 21:04:55.000000 oceanum-0.8.2/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:46:33.028474 oceanum-0.8.2/tests/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-14 22:31:40.000000 oceanum-0.8.2/tests/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-07-31 20:46:33.032474 oceanum-0.8.2/tests/data/
+-rw-rw-r--   0 dave      (1000) dave      (1000)    21010 2023-05-14 22:31:40.000000 oceanum-0.8.2/tests/data/grid_data_1.nc
+-rw-rw-r--   0 dave      (1000) dave      (1000)  2029589 2023-05-14 22:31:40.000000 oceanum-0.8.2/tests/data/ocean_test_1.mp4
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1727 2023-05-14 22:31:40.000000 oceanum-0.8.2/tests/data/point_data_1.csv
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1222 2023-05-14 22:31:40.000000 oceanum-0.8.2/tests/test_catalog.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1072 2023-05-14 22:31:40.000000 oceanum-0.8.2/tests/test_datamesh_connect.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1643 2023-05-14 22:31:40.000000 oceanum-0.8.2/tests/test_datamesh_load.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2578 2023-05-14 22:31:40.000000 oceanum-0.8.2/tests/test_datamesh_query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3255 2023-05-14 22:31:40.000000 oceanum-0.8.2/tests/test_datamesh_write.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2958 2023-07-11 22:58:57.000000 oceanum-0.8.2/tests/test_datasource.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1482 2023-07-11 23:07:04.000000 oceanum-0.8.2/tests/test_query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      805 2023-05-14 22:31:40.000000 oceanum-0.8.2/tests/test_video_compat.py
```

### Comparing `oceanum-0.8.1/CONTRIBUTING.rst` & `oceanum-0.8.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/LICENSE` & `oceanum-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/PKG-INFO` & `oceanum-0.8.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanum
-Version: 0.8.1
+Version: 0.8.2
 Summary: Library for oceanum.io services
 Home-page: https://github.com/oceanum/oceanum-python
 Author: Oceanum Developers
 Author-email: developers@oceanum.science
 License: MIT license
 Keywords: oceanum
 License-File: LICENSE
```

### Comparing `oceanum-0.8.1/README.rst` & `oceanum-0.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/docs/Makefile` & `oceanum-0.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/docs/api.rst` & `oceanum-0.8.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/docs/classes/datamesh/oceanum.datamesh.Connector.rst` & `oceanum-0.8.2/docs/classes/datamesh/oceanum.datamesh.Connector.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/docs/conf.py` & `oceanum-0.8.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/docs/index.rst` & `oceanum-0.8.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/docs/installation.rst` & `oceanum-0.8.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/docs/make.bat` & `oceanum-0.8.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/docs/oceanum.datamesh.rst` & `oceanum-0.8.2/docs/oceanum.datamesh.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/docs/usage.rst` & `oceanum-0.8.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/oceanum/datamesh/catalog.py` & `oceanum-0.8.2/oceanum/datamesh/catalog.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/oceanum/datamesh/connection.py` & `oceanum-0.8.2/oceanum/datamesh/connection.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/oceanum/datamesh/datasource.py` & `oceanum-0.8.2/oceanum/datamesh/datasource.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/oceanum/datamesh/query.py` & `oceanum-0.8.2/oceanum/datamesh/query.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/oceanum/datamesh/zarr.py` & `oceanum-0.8.2/oceanum/datamesh/zarr.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/oceanum.egg-info/PKG-INFO` & `oceanum-0.8.2/oceanum.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanum
-Version: 0.8.1
+Version: 0.8.2
 Summary: Library for oceanum.io services
 Home-page: https://github.com/oceanum/oceanum-python
 Author: Oceanum Developers
 Author-email: developers@oceanum.science
 License: MIT license
 Keywords: oceanum
 License-File: LICENSE
```

### Comparing `oceanum-0.8.1/oceanum.egg-info/SOURCES.txt` & `oceanum-0.8.2/oceanum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/setup.py` & `oceanum-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/tests/data/grid_data_1.nc` & `oceanum-0.8.2/tests/data/grid_data_1.nc`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/tests/data/ocean_test_1.mp4` & `oceanum-0.8.2/tests/data/ocean_test_1.mp4`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/tests/data/point_data_1.csv` & `oceanum-0.8.2/tests/data/point_data_1.csv`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/tests/test_catalog.py` & `oceanum-0.8.2/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/tests/test_datamesh_connect.py` & `oceanum-0.8.2/tests/test_datamesh_connect.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/tests/test_datamesh_load.py` & `oceanum-0.8.2/tests/test_datamesh_load.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/tests/test_datamesh_query.py` & `oceanum-0.8.2/tests/test_datamesh_query.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/tests/test_datamesh_write.py` & `oceanum-0.8.2/tests/test_datamesh_write.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/tests/test_datasource.py` & `oceanum-0.8.2/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/tests/test_query.py` & `oceanum-0.8.2/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.8.1/tests/test_video_compat.py` & `oceanum-0.8.2/tests/test_video_compat.py`

 * *Files identical despite different names*

