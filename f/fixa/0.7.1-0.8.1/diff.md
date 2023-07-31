# Comparing `tmp/fixa-0.7.1.tar.gz` & `tmp/fixa-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixa-0.7.1.tar", last modified: Sat May 27 19:11:38 2023, max compression
+gzip compressed data, was "fixa-0.8.1.tar", last modified: Mon Jul 31 00:06:08 2023, max compression
```

## Comparing `fixa-0.7.1.tar` & `fixa-0.8.1.tar`

### file list

```diff
@@ -1,54 +1,61 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-27 19:11:38.085145 fixa-0.7.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-06 00:03:13.000000 fixa-0.7.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1114 2023-05-06 00:03:13.000000 fixa-0.7.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      312 2023-05-06 00:03:13.000000 fixa-0.7.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-05-27 19:11:38.084988 fixa-0.7.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     2986 2023-05-06 00:03:13.000000 fixa-0.7.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-27 19:11:38.062302 fixa-0.7.1/fixa/
--rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-05-06 00:03:13.000000 fixa-0.7.1/fixa/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-27 19:11:06.000000 fixa-0.7.1/fixa/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4137 2023-05-08 06:09:51.000000 fixa-0.7.1/fixa/better_enum.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      650 2023-05-27 18:21:44.000000 fixa-0.7.1/fixa/better_pathlib.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6675 2023-05-06 00:03:13.000000 fixa-0.7.1/fixa/binarysearch.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3225 2023-05-26 17:28:21.000000 fixa-0.7.1/fixa/build_dist.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1333 2023-05-06 03:12:23.000000 fixa-0.7.1/fixa/dataclass_dataframe.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-27 19:11:38.081551 fixa-0.7.1/fixa/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-06 00:03:13.000000 fixa-0.7.1/fixa/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2998 2023-05-27 18:40:26.000000 fixa-0.7.1/fixa/git_cli.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-05-27 18:23:51.000000 fixa-0.7.1/fixa/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    12219 2023-05-06 01:55:53.000000 fixa-0.7.1/fixa/iterable.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    17911 2023-05-12 16:53:54.000000 fixa-0.7.1/fixa/nest_logger.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       82 2023-05-27 18:41:51.000000 fixa-0.7.1/fixa/nested_logger.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      469 2023-05-06 03:18:07.000000 fixa-0.7.1/fixa/os_platform.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-06 05:18:39.000000 fixa-0.7.1/fixa/pytest_cov_helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3145 2023-05-06 01:57:52.000000 fixa-0.7.1/fixa/rnd.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1933 2023-05-06 03:17:46.000000 fixa-0.7.1/fixa/runtime.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-27 19:11:38.081858 fixa-0.7.1/fixa/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      539 2023-05-06 05:18:39.000000 fixa-0.7.1/fixa/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4757 2023-05-06 00:03:13.000000 fixa-0.7.1/fixa/timer.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-27 19:11:38.063067 fixa-0.7.1/fixa.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-05-27 19:11:38.000000 fixa-0.7.1/fixa.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      945 2023-05-27 19:11:38.000000 fixa-0.7.1/fixa.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-27 19:11:38.000000 fixa-0.7.1/fixa.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-05-27 19:11:38.000000 fixa-0.7.1/fixa.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        5 2023-05-27 19:11:38.000000 fixa-0.7.1/fixa.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      706 2023-05-26 17:22:09.000000 fixa-0.7.1/pyproject.toml
--rw-r--r--   0 sanhehu    (501) staff       (20)     2889 2023-05-27 18:40:37.000000 fixa-0.7.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      295 2023-05-06 00:03:13.000000 fixa-0.7.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-26 17:19:20.000000 fixa-0.7.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-05-06 00:03:13.000000 fixa-0.7.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-05-06 00:03:13.000000 fixa-0.7.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-27 19:11:38.085189 fixa-0.7.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7699 2023-05-06 00:03:13.000000 fixa-0.7.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-27 19:11:38.084690 fixa-0.7.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     3858 2023-05-08 05:53:35.000000 fixa-0.7.1/tests/test_better_enum.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      758 2023-05-27 18:22:18.000000 fixa-0.7.1/tests/test_better_pathlib.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1633 2023-05-06 01:48:18.000000 fixa-0.7.1/tests/test_binarysearch.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      692 2023-05-06 01:42:50.000000 fixa-0.7.1/tests/test_dataclass_dataframe.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      926 2023-05-27 18:39:25.000000 fixa-0.7.1/tests/test_git_cli.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2892 2023-05-27 18:21:55.000000 fixa-0.7.1/tests/test_hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      214 2023-05-06 01:48:59.000000 fixa-0.7.1/tests/test_import.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6529 2023-05-06 01:56:07.000000 fixa-0.7.1/tests/test_iterable.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4127 2023-05-12 03:29:46.000000 fixa-0.7.1/tests/test_nest_logger.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      661 2023-05-06 01:58:16.000000 fixa-0.7.1/tests/test_rnd.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3432 2023-05-06 02:03:21.000000 fixa-0.7.1/tests/test_timer.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-31 00:06:08.150102 fixa-0.8.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-06 00:03:13.000000 fixa-0.8.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1114 2023-05-06 00:03:13.000000 fixa-0.8.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      312 2023-05-06 00:03:13.000000 fixa-0.8.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-07-31 00:06:08.149943 fixa-0.8.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2986 2023-05-06 00:03:13.000000 fixa-0.8.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-31 00:06:08.144633 fixa-0.8.1/fixa/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-05-06 00:03:13.000000 fixa-0.8.1/fixa/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-30 23:54:27.000000 fixa-0.8.1/fixa/_version.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-31 00:06:08.146411 fixa-0.8.1/fixa/aws/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-05-29 01:36:28.000000 fixa-0.8.1/fixa/aws/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    13347 2023-07-30 23:49:46.000000 fixa-0.8.1/fixa/aws/aws_dynamodb_export_to_s3.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4232 2023-07-31 00:03:30.000000 fixa-0.8.1/fixa/aws/aws_s3_uri.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-05-29 01:49:30.000000 fixa-0.8.1/fixa/aws/mock_test.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4137 2023-05-08 06:09:51.000000 fixa-0.8.1/fixa/better_enum.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      650 2023-05-27 18:21:44.000000 fixa-0.8.1/fixa/better_pathlib.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6675 2023-05-06 00:03:13.000000 fixa-0.8.1/fixa/binarysearch.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3225 2023-05-26 17:28:21.000000 fixa-0.8.1/fixa/build_dist.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1333 2023-05-06 03:12:23.000000 fixa-0.8.1/fixa/dataclass_dataframe.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-31 00:06:08.146617 fixa-0.8.1/fixa/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-06 00:03:13.000000 fixa-0.8.1/fixa/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2998 2023-05-27 18:40:26.000000 fixa-0.8.1/fixa/git_cli.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-05-27 18:23:51.000000 fixa-0.8.1/fixa/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    13674 2023-06-06 13:40:37.000000 fixa-0.8.1/fixa/iterable.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    17911 2023-05-12 16:53:54.000000 fixa-0.8.1/fixa/nest_logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       82 2023-05-27 18:41:51.000000 fixa-0.8.1/fixa/nested_logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      469 2023-05-06 03:18:07.000000 fixa-0.8.1/fixa/os_platform.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-05-06 05:18:39.000000 fixa-0.8.1/fixa/pytest_cov_helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3145 2023-05-06 01:57:52.000000 fixa-0.8.1/fixa/rnd.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1933 2023-05-06 03:17:46.000000 fixa-0.8.1/fixa/runtime.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-31 00:06:08.146857 fixa-0.8.1/fixa/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      539 2023-05-06 05:18:39.000000 fixa-0.8.1/fixa/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4757 2023-05-06 00:03:13.000000 fixa-0.8.1/fixa/timer.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2332 2023-06-03 20:12:06.000000 fixa-0.8.1/fixa/waiter.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-31 00:06:08.145512 fixa-0.8.1/fixa.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4095 2023-07-31 00:06:08.000000 fixa-0.8.1/fixa.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1085 2023-07-31 00:06:08.000000 fixa-0.8.1/fixa.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-31 00:06:08.000000 fixa-0.8.1/fixa.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-07-31 00:06:08.000000 fixa-0.8.1/fixa.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        5 2023-07-31 00:06:08.000000 fixa-0.8.1/fixa.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      706 2023-05-26 17:22:09.000000 fixa-0.8.1/pyproject.toml
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3201 2023-07-31 00:04:08.000000 fixa-0.8.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      295 2023-05-06 00:03:13.000000 fixa-0.8.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-26 17:19:20.000000 fixa-0.8.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      183 2023-05-06 00:03:13.000000 fixa-0.8.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        0 2023-05-06 00:03:13.000000 fixa-0.8.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-31 00:06:08.150156 fixa-0.8.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7699 2023-05-06 00:03:13.000000 fixa-0.8.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-31 00:06:08.149625 fixa-0.8.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3858 2023-05-08 05:53:35.000000 fixa-0.8.1/tests/test_better_enum.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      758 2023-05-27 18:22:18.000000 fixa-0.8.1/tests/test_better_pathlib.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1633 2023-05-06 01:48:18.000000 fixa-0.8.1/tests/test_binarysearch.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      692 2023-05-06 01:42:50.000000 fixa-0.8.1/tests/test_dataclass_dataframe.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      926 2023-05-27 18:39:25.000000 fixa-0.8.1/tests/test_git_cli.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2892 2023-05-27 18:21:55.000000 fixa-0.8.1/tests/test_hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      214 2023-05-06 01:48:59.000000 fixa-0.8.1/tests/test_import.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7295 2023-07-30 23:57:28.000000 fixa-0.8.1/tests/test_iterable.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4127 2023-05-12 03:29:46.000000 fixa-0.8.1/tests/test_nest_logger.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      661 2023-05-06 01:58:16.000000 fixa-0.8.1/tests/test_rnd.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3432 2023-05-06 02:03:21.000000 fixa-0.8.1/tests/test_timer.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      833 2023-06-03 20:13:04.000000 fixa-0.8.1/tests/test_waiter.py
```

### Comparing `fixa-0.7.1/LICENSE.txt` & `fixa-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/PKG-INFO` & `fixa-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fixa
-Version: 0.7.1
+Version: 0.8.1
 Summary: Like the Ikea FIXA, it is my toolbox to fix things.
 Home-page: https://github.com/MacHu-GWU/fixa-project
-Download-URL: https://pypi.python.org/pypi/fixa/0.7.1#downloads
+Download-URL: https://pypi.python.org/pypi/fixa/0.8.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `fixa-0.7.1/README.rst` & `fixa-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/fixa/better_enum.py` & `fixa-0.8.1/fixa/better_enum.py`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/fixa/better_pathlib.py` & `fixa-0.8.1/fixa/better_pathlib.py`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/fixa/binarysearch.py` & `fixa-0.8.1/fixa/binarysearch.py`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/fixa/build_dist.py` & `fixa-0.8.1/fixa/build_dist.py`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/fixa/dataclass_dataframe.py` & `fixa-0.8.1/fixa/dataclass_dataframe.py`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/fixa/git_cli.py` & `fixa-0.8.1/fixa/git_cli.py`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/fixa/hashes.py` & `fixa-0.8.1/fixa/hashes.py`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/fixa/iterable.py` & `fixa-0.8.1/fixa/iterable.py`

 * *Files 10% similar despite different names*

```diff
@@ -494,7 +494,58 @@
         raise ValueError()
     if k < 0:
         raise ValueError("k has to be greater or equal than zero!")
     elif k == 0:
         return [i - i for i in array]
     else:
         return [j - i for i, j in zip(array[:-k], array[k:])]
+
+
+KT = T.TypeVar("KT")
+VT = T.TypeVar("VT")
+
+def group_by(
+    iterable: T.Iterable[VT],
+    get_key: T.Callable[[VT], KT],
+) -> T.Dict[KT, T.List[VT]]:
+    """
+    Group items by it's key, with type hint.
+
+    Example::
+
+        >>> class Record:
+        ...     def __init__(self, product: str, date: str, sale: int):
+        ...         self.product = product
+        ...         self.date = date
+        ...         self.sale = sale
+
+        >>> records = [
+        ...     Record("apple", "2020-01-01", 10),
+        ...     Record("apple", "2020-01-02", 20),
+        ...     Record("apple", "2020-01-03", 30),
+        ...     Record("banana", "2020-01-01", 10),
+        ...     Record("banana", "2020-01-02", 20),
+        ...     Record("banana", "2020-01-03", 30),
+        ... ]
+
+        >>> group_by(records, lambda x: x.product)
+        {
+            "apple": [
+                Record("apple", "2020-01-01", 10),
+                Record("apple", "2020-01-02", 20),
+                Record("apple", "2020-01-03", 30),
+            ],
+            "banana": [
+                Record("banana", "2020-01-01", 10),
+                Record("banana", "2020-01-02", 20),
+                Record("banana", "2020-01-03", 30),
+            ],
+        }
+    """
+    grouped = dict()
+    for item in iterable:
+        key = get_key(item)
+        try:
+            grouped[key].append(item)
+        except KeyError:
+            grouped[key] = [item]
+    return grouped
```

### Comparing `fixa-0.7.1/fixa/nest_logger.py` & `fixa-0.8.1/fixa/nest_logger.py`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/fixa/pytest_cov_helper.py` & `fixa-0.8.1/fixa/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/fixa/rnd.py` & `fixa-0.8.1/fixa/rnd.py`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/fixa/runtime.py` & `fixa-0.8.1/fixa/runtime.py`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/fixa/tests/__init__.py` & `fixa-0.8.1/fixa/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/fixa/timer.py` & `fixa-0.8.1/fixa/timer.py`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/fixa.egg-info/PKG-INFO` & `fixa-0.8.1/fixa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fixa
-Version: 0.7.1
+Version: 0.8.1
 Summary: Like the Ikea FIXA, it is my toolbox to fix things.
 Home-page: https://github.com/MacHu-GWU/fixa-project
-Download-URL: https://pypi.python.org/pypi/fixa/0.7.1#downloads
+Download-URL: https://pypi.python.org/pypi/fixa/0.8.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `fixa-0.7.1/pyproject.toml` & `fixa-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/release-history.rst` & `fixa-0.8.1/release-history.rst`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,24 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.8.1 (2023-07-31)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- add ``waiter.Waiter`` for retry and long polling pattern
+- add ``iterable.group_by`` function
+- add ``aws.aws_s3_uri.py`` module
+- add ``aws.aws_dynamodb_export_to_s3.py`` module
+
+
 0.7.1 (2023-05-27)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - add ``hashes.Hashes.of_folder`` and ``hashes.Hashes.of_paths``.
 - add ``git_cli.locate_dir_repo``.
```

### Comparing `fixa-0.7.1/requirements-doc.txt` & `fixa-0.8.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/setup.py` & `fixa-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/tests/test_better_enum.py` & `fixa-0.8.1/tests/test_better_enum.py`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/tests/test_better_pathlib.py` & `fixa-0.8.1/tests/test_better_pathlib.py`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/tests/test_binarysearch.py` & `fixa-0.8.1/tests/test_binarysearch.py`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/tests/test_dataclass_dataframe.py` & `fixa-0.8.1/tests/test_dataclass_dataframe.py`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/tests/test_git_cli.py` & `fixa-0.8.1/tests/test_git_cli.py`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/tests/test_hashes.py` & `fixa-0.8.1/tests/test_hashes.py`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/tests/test_iterable.py` & `fixa-0.8.1/tests/test_iterable.py`

 * *Files 7% similar despite different names*

```diff
@@ -108,14 +108,40 @@
     assert list(iterable.grouper_dict(d, 2)) == [
         {"a": 1, "b": 2},
         {"c": 3, "d": 4},
         {"e": 5},
     ]
 
 
+def test_group_by():
+    class Record:
+        def __init__(self, product: str, date: str, sale: int):
+            self.product = product
+            self.date = date
+            self.sale = sale
+
+    records = [
+        Record("apple", "2020-01-01", 10),
+        Record("apple", "2020-01-02", 20),
+        Record("apple", "2020-01-03", 30),
+        Record("banana", "2020-01-01", 10),
+        Record("banana", "2020-01-02", 20),
+        Record("banana", "2020-01-03", 30),
+    ]
+
+    groups = iterable.group_by(records, get_key=lambda x: x.product)
+
+    sales = [record.sale for record in groups["apple"]]
+    sales.sort()
+    assert sales == [10, 20, 30]
+    sales = [record.sale for record in groups["banana"]]
+    sales.sort()
+    assert sales == [10, 20, 30]
+
+
 def test_size_of_generator():
     """测试 :func:`~sfm.iterable.size_of_generator`  的性能。"""
 
     def number_generator():
         for i in range(1000 * 1000):
             yield i
```

### Comparing `fixa-0.7.1/tests/test_nest_logger.py` & `fixa-0.8.1/tests/test_nest_logger.py`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/tests/test_rnd.py` & `fixa-0.8.1/tests/test_rnd.py`

 * *Files identical despite different names*

### Comparing `fixa-0.7.1/tests/test_timer.py` & `fixa-0.8.1/tests/test_timer.py`

 * *Files identical despite different names*

