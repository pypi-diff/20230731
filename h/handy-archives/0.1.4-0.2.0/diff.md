# Comparing `tmp/handy-archives-0.1.4.tar.gz` & `tmp/handy_archives-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "handy-archives-0.1.4.tar", last modified: Sat May 14 09:07:53 2022, max compression
+gzip compressed data, was "handy_archives-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `handy-archives-0.1.4.tar` & `handy_archives-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2022-05-14 09:07:20.020811 handy-archives-0.1.4/LICENSE
--rw-r--r--   0        0        0     5341 2022-05-14 09:07:20.020811 handy-archives-0.1.4/README.rst
--rw-r--r--   0        0        0    10536 2022-05-14 09:07:20.020811 handy-archives-0.1.4/handy_archives/__init__.py
--rw-r--r--   0        0        0        0 2022-05-14 09:07:20.020811 handy-archives-0.1.4/handy_archives/py.typed
--rw-r--r--   0        0        0     3167 2022-05-14 09:07:20.020811 handy-archives-0.1.4/handy_archives/testing.py
--rw-r--r--   0        0        0     4920 2022-05-14 09:07:20.020811 handy-archives-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     7026 1970-01-01 00:00:00.000000 handy-archives-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-31 14:38:09.756028 handy_archives-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5343 2023-07-31 14:38:09.756028 handy_archives-0.2.0/README.rst
+-rw-r--r--   0        0        0    12411 2023-07-31 14:38:09.756028 handy_archives-0.2.0/handy_archives/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 14:38:09.756028 handy_archives-0.2.0/handy_archives/py.typed
+-rw-r--r--   0        0        0     3167 2023-07-31 14:38:09.756028 handy_archives-0.2.0/handy_archives/testing.py
+-rw-r--r--   0        0        0     4974 2023-07-31 14:38:09.756028 handy_archives-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7079 1970-01-01 00:00:00.000000 handy_archives-0.2.0/PKG-INFO
```

### Comparing `handy-archives-0.1.4/LICENSE` & `handy_archives-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `handy-archives-0.1.4/README.rst` & `handy_archives-0.2.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 	:target: https://github.com/domdfcoding/handy-archives/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/domdfcoding/handy-archives/workflows/mypy/badge.svg
 	:target: https://github.com/domdfcoding/handy-archives/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/handy-archives/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/handy-archives/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/handy-archives/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/handy-archives/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/handy-archives/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/handy-archives?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/handy-archives?logo=codefactor
@@ -97,23 +97,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/handy-archives
 	:target: https://github.com/domdfcoding/handy-archives/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/handy-archives
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/handy-archives/v0.1.4
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/handy-archives/v0.2.0
 	:target: https://github.com/domdfcoding/handy-archives/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/handy-archives
 	:target: https://github.com/domdfcoding/handy-archives/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/handy-archives
 	:target: https://pypi.org/project/handy-archives/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `handy-archives-0.1.4/handy_archives/__init__.py` & `handy_archives-0.2.0/handy_archives/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,34 +30,51 @@
 import datetime
 import os
 import pathlib
 import shutil
 import sys
 import tarfile
 import zipfile
-from typing import IO, Optional, Type, TypeVar, Union, cast
+from typing import IO, TYPE_CHECKING, Callable, Iterable, Optional, Type, TypeVar, Union, cast, no_type_check
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2021 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.1.4"
+__version__: str = "0.2.0"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = ["unpack_archive", "TarFile", "ZipFile", "is_tarfile"]
 
 _Self = TypeVar("_Self")
 PathLike = Union[str, pathlib.Path, os.PathLike]
 
 if "wheel" not in shutil._UNPACK_FORMATS:  # type: ignore[attr-defined]
 	shutil.register_unpack_format(
 			name="wheel",
 			extensions=[".whl"],
 			function=shutil._unpack_zipfile,  # type: ignore[attr-defined]
 			)
 
+if TYPE_CHECKING or not hasattr(tarfile, "FilterError"):  # pragma: nocover
+
+	def fully_trusted_filter(member, dest_path):  # noqa: MAN001,MAN002
+		return member
+
+	def tar_filter(member, dest_path):  # noqa: MAN001,MAN002
+		return member
+
+	def data_filter(member, dest_path):  # noqa: MAN001,MAN002
+		return member
+
+else:  # pragma: nocover
+	# stdlib
+	from tarfile import data_filter as data_filter
+	from tarfile import fully_trusted_filter as fully_trusted_filter
+	from tarfile import tar_filter as tar_filter
+
 
 def unpack_archive(
 		filename: PathLike,
 		extract_dir: Optional[PathLike] = None,
 		format: Optional[str] = None,  # noqa: A002  # pylint: disable=redefined-builtin
 		) -> None:
 	"""
@@ -90,14 +107,62 @@
 	"""
 	Subclass of :class:`tarfile.TarFile` with additional methods.
 	"""
 
 	closed: bool
 	offset: int
 
+	@no_type_check
+	def extractall(
+			self,
+			path: PathLike = '.',
+			members: Optional[Iterable[tarfile.TarInfo]] = None,
+			*,
+			numeric_owner: bool = False,
+			filter: Optional[Callable] = None,  # noqa: A002  # pylint: disable=redefined-builtin
+			) -> None:  # pragma: nocover
+		"""
+		Wrapper around :meth:`tarfile.TarFile.extractall` with compatibility shim for :pep:`706` on unpatched Pythons.
+		"""
+
+		if hasattr(tarfile, "FilterError"):
+			return super().extractall(
+					path,
+					members,
+					numeric_owner=numeric_owner,
+					filter=filter,
+					)
+		else:
+			return super().extractall(path, members, numeric_owner=numeric_owner)
+
+	@no_type_check
+	def extract(
+			self,
+			member: Union[str, tarfile.TarInfo],
+			path: PathLike = '',
+			set_attrs: bool = True,
+			*,
+			numeric_owner: bool = False,
+			filter: Optional[Callable] = None,  # noqa: A002  # pylint: disable=redefined-builtin
+			) -> None:  # pragma: nocover
+		"""
+		Wrapper around :meth:`tarfile.TarFile.extract` with compatibility shim for :pep:`706` on unpatched Pythons.
+		"""
+
+		if hasattr(tarfile, "FilterError"):
+			return super().extract(
+					member,
+					path,
+					set_attrs,
+					numeric_owner=numeric_owner,
+					filter=filter,
+					)
+		else:
+			return super().extract(member, path, set_attrs, numeric_owner=numeric_owner)
+
 	def extractfile(self, member: Union[str, tarfile.TarInfo]) -> IO[bytes]:
 		"""
 		Extract a member from the archive as a file object.
 
 		:param member: A filename or a :class:`tarfile.TarInfo` object.
 
 		If ``member`` is a regular file or a link, an :class:`io.BufferedReader` object is returned.
```

### Comparing `handy-archives-0.1.4/handy_archives/testing.py` & `handy_archives-0.2.0/handy_archives/testing.py`

 * *Files identical despite different names*

### Comparing `handy-archives-0.1.4/pyproject.toml` & `handy_archives-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "flit-core<4,>=3.2",]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "handy-archives"
-version = "0.1.4"
+version = "0.2.0"
 description = "Some handy archive helpers for Python."
 readme = "README.rst"
 requires-python = ">=3.6.1"
 keywords = [ "archive", "shutil", "tar", "zip",]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -17,14 +17,15 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Archiving",
     "Topic :: System :: Archiving :: Compression",
     "Typing :: Typed",
 ]
@@ -141,15 +142,15 @@
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Archiving",
     "Topic :: System :: Archiving :: Compression",
     "Typing :: Typed",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 package = "handy_archives"
 
 [tool.mypy]
 python_version = "3.7"
```

### Comparing `handy-archives-0.1.4/PKG-INFO` & `handy_archives-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: handy-archives
-Version: 0.1.4
+Version: 0.2.0
 Summary: Some handy archive helpers for Python.
 Keywords: archive,shutil,tar,zip
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 Requires-Python: >=3.6.1
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: System :: Archiving :: Compression
 Classifier: Typing :: Typed
 Requires-Dist: coincidence>=0.2.0 ; extra == "all"
@@ -90,16 +91,16 @@
 	:target: https://github.com/domdfcoding/handy-archives/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/domdfcoding/handy-archives/workflows/mypy/badge.svg
 	:target: https://github.com/domdfcoding/handy-archives/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/handy-archives/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/handy-archives/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/handy-archives/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/handy-archives/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/handy-archives/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/handy-archives?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/handy-archives?logo=codefactor
@@ -133,23 +134,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/handy-archives
 	:target: https://github.com/domdfcoding/handy-archives/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/handy-archives
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/handy-archives/v0.1.4
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/handy-archives/v0.2.0
 	:target: https://github.com/domdfcoding/handy-archives/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/handy-archives
 	:target: https://github.com/domdfcoding/handy-archives/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/handy-archives
 	:target: https://pypi.org/project/handy-archives/
 	:alt: PyPI - Downloads
 
 .. end shields
```

