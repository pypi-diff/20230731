# Comparing `tmp/attr_utils-0.8.1.tar.gz` & `tmp/attr_utils-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attr_utils-0.8.1.tar", last modified: Fri Jul 21 12:59:20 2023, max compression
+gzip compressed data, was "attr_utils-0.9.0.tar", last modified: Mon Jul 31 14:53:10 2023, max compression
```

## Comparing `attr_utils-0.8.1.tar` & `attr_utils-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-07-21 12:59:20.013534 attr_utils-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-21 12:59:20.021534 attr_utils-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     5325 2023-07-21 12:59:20.021534 attr_utils-0.8.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7299 2023-07-21 12:59:20.025534 attr_utils-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5000 2023-07-21 12:59:20.021534 attr_utils-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     4206 2023-07-21 12:58:43.940897 attr_utils-0.8.1/attr_utils/docstrings.py
--rw-r--r--   0 runner    (1001) docker     (122)     6609 2023-07-21 12:58:43.940897 attr_utils-0.8.1/attr_utils/serialise.py
--rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-07-21 12:58:43.940897 attr_utils-0.8.1/attr_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8224 2023-07-21 12:58:43.940897 attr_utils-0.8.1/attr_utils/mypy_plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)     8713 2023-07-21 12:58:43.940897 attr_utils-0.8.1/attr_utils/annotations.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 12:58:43.940897 attr_utils-0.8.1/attr_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     6047 2023-07-21 12:58:43.940897 attr_utils-0.8.1/attr_utils/pprinter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1707 2023-07-21 12:58:43.940897 attr_utils-0.8.1/attr_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12328 2023-07-21 12:58:43.940897 attr_utils-0.8.1/attr_utils/autoattrs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-07-31 14:53:10.092008 attr_utils-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-31 14:53:10.100008 attr_utils-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5325 2023-07-31 14:53:10.100008 attr_utils-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7289 2023-07-31 14:53:10.104008 attr_utils-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4990 2023-07-31 14:53:10.100008 attr_utils-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-07-31 14:52:34.035780 attr_utils-0.9.0/attr_utils/docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6609 2023-07-31 14:52:34.035780 attr_utils-0.9.0/attr_utils/serialise.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-07-31 14:52:34.031780 attr_utils-0.9.0/attr_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8224 2023-07-31 14:52:34.035780 attr_utils-0.9.0/attr_utils/mypy_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8793 2023-07-31 14:52:34.031780 attr_utils-0.9.0/attr_utils/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 14:52:34.035780 attr_utils-0.9.0/attr_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     6047 2023-07-31 14:52:34.035780 attr_utils-0.9.0/attr_utils/pprinter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1707 2023-07-31 14:52:34.035780 attr_utils-0.9.0/attr_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12736 2023-07-31 14:52:34.035780 attr_utils-0.9.0/attr_utils/autoattrs.py
```

### Comparing `attr_utils-0.8.1/LICENSE` & `attr_utils-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `attr_utils-0.8.1/README.rst` & `attr_utils-0.9.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/attr_utils
 	:target: https://github.com/domdfcoding/attr_utils/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/attr_utils
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/attr_utils/v0.8.1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/attr_utils/v0.9.0
 	:target: https://github.com/domdfcoding/attr_utils/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/attr_utils
 	:target: https://github.com/domdfcoding/attr_utils/commit/master
 	:alt: GitHub last commit
```

### Comparing `attr_utils-0.8.1/PKG-INFO` & `attr_utils-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attr-utils
-Version: 0.8.1
+Version: 0.9.0
 Summary: Utilities to augment attrs.
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: attrs,documentation,serde,sphinx
 Home-page: https://github.com/domdfcoding/attr_utils
 Project-URL: Issue Tracker, https://github.com/domdfcoding/attr_utils/issues
 Project-URL: Source Code, https://github.com/domdfcoding/attr_utils
@@ -24,24 +24,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
-Requires-Dist: attrs>=19.3.0
-Requires-Dist: domdf-python-tools>=2.9.0
+Requires-Dist: attrs>=21.2.0
+Requires-Dist: domdf-python-tools>=3.6.1
 Requires-Dist: toolz>=0.11.1
-Requires-Dist: typing-extensions>=3.7.4.3
+Requires-Dist: typing-extensions>=4.0.0
 Requires-Dist: typing-inspect>=0.6.0; python_version == "3.6"
 Requires-Dist: prettyprinter==0.18.0; extra == 'pprint'
-Requires-Dist: sphinx<3.4.0,>=3.2.0; extra == 'sphinx'
+Requires-Dist: sphinx<5,>=3.2.0; extra == 'sphinx'
 Requires-Dist: sphinx-toolbox>=2.16.0; extra == 'sphinx'
 Requires-Dist: prettyprinter==0.18.0; extra == 'all'
-Requires-Dist: sphinx<3.4.0,>=3.2.0; extra == 'all'
+Requires-Dist: sphinx<5,>=3.2.0; extra == 'all'
 Requires-Dist: sphinx-toolbox>=2.16.0; extra == 'all'
 Provides-Extra: pprint
 Provides-Extra: sphinx
 Provides-Extra: all
 Description-Content-Type: text/x-rst
 
 
@@ -144,15 +144,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/attr_utils
 	:target: https://github.com/domdfcoding/attr_utils/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/attr_utils
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/attr_utils/v0.8.1
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/attr_utils/v0.9.0
 	:target: https://github.com/domdfcoding/attr_utils/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/attr_utils
 	:target: https://github.com/domdfcoding/attr_utils/commit/master
 	:alt: GitHub last commit
```

### Comparing `attr_utils-0.8.1/pyproject.toml` & `attr_utils-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "attr_utils"
-version = "0.8.1"
+version = "0.9.0"
 description = "Utilities to augment attrs."
 readme = "README.rst"
 keywords = [ "attrs", "documentation", "serde", "sphinx",]
 dynamic = []
 dependencies = [
-    "attrs>=19.3.0",
-    "domdf-python-tools>=2.9.0",
+    "attrs>=21.2.0",
+    "domdf-python-tools>=3.6.1",
     "toolz>=0.11.1",
-    "typing-extensions>=3.7.4.3",
+    "typing-extensions>=4.0.0",
     'typing-inspect>=0.6.0; python_version == "3.6"',
 ]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
@@ -47,16 +47,16 @@
 Homepage = "https://github.com/domdfcoding/attr_utils"
 "Issue Tracker" = "https://github.com/domdfcoding/attr_utils/issues"
 "Source Code" = "https://github.com/domdfcoding/attr_utils"
 Documentation = "https://attr-utils.readthedocs.io/en/latest"
 
 [project.optional-dependencies]
 pprint = [ "prettyprinter==0.18.0",]
-sphinx = [ "sphinx<3.4.0,>=3.2.0", "sphinx-toolbox>=2.16.0",]
-all = [ "prettyprinter==0.18.0", "sphinx<3.4.0,>=3.2.0", "sphinx-toolbox>=2.16.0",]
+sphinx = [ "sphinx<5,>=3.2.0", "sphinx-toolbox>=2.16.0",]
+all = [ "prettyprinter==0.18.0", "sphinx<5,>=3.2.0", "sphinx-toolbox>=2.16.0",]
 
 [tool.mkrecipe]
 conda-channels = [ "conda-forge", "domdfcoding",]
 extras = "all"
 license-key = "MIT"
 
 [tool.sphinx-pyproject]
```

### Comparing `attr_utils-0.8.1/attr_utils/docstrings.py` & `attr_utils-0.9.0/attr_utils/docstrings.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 # stdlib
 import re
 import sys
 from types import MethodType
 from typing import Optional, Pattern, Type, TypeVar
 
 # 3rd party
-from domdf_python_tools.compat import PYPY, PYPY37
+from domdf_python_tools.compat import PYPY
 from domdf_python_tools.doctools import base_new_docstrings, prettify_docstrings
 from domdf_python_tools.typing import MethodDescriptorType, MethodWrapperType, WrapperDescriptorType
 
 __all__ = ["add_attrs_doc", "_T"]
 
 attrs_docstring = "Automatically created by attrs."
 ne_default = "Check equality and either forward a NotImplemented or return the result\n    negated."
```

### Comparing `attr_utils-0.8.1/attr_utils/serialise.py` & `attr_utils-0.9.0/attr_utils/serialise.py`

 * *Files identical despite different names*

### Comparing `attr_utils-0.8.1/attr_utils/__init__.py` & `attr_utils-0.9.0/attr_utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,11 +25,11 @@
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.8.1"
+__version__: str = "0.9.0"
 __email__: str = "dominic@davis-foster.co.uk"
 
 _docs = False
```

### Comparing `attr_utils-0.8.1/attr_utils/mypy_plugin.py` & `attr_utils-0.9.0/attr_utils/mypy_plugin.py`

 * *Files identical despite different names*

### Comparing `attr_utils-0.8.1/attr_utils/annotations.py` & `attr_utils-0.9.0/attr_utils/annotations.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,17 @@
 
 	.. _attrs: https://www.attrs.org/en/stable/
 	"""
 
 	if not attr.has(obj):  # type: ignore
 		return obj
 
+	if hasattr(obj, "__attrs_init__"):
+		return obj  # type: ignore[return-value]
+
 	annotations: Dict[str, Optional[Type]] = {"return": None}
 
 	attrs = attr.fields(obj)
 
 	for a in attrs:
 		arg_name = a.name.lstrip('_')
```

### Comparing `attr_utils-0.8.1/attr_utils/pprinter.py` & `attr_utils-0.9.0/attr_utils/pprinter.py`

 * *Files identical despite different names*

### Comparing `attr_utils-0.8.1/attr_utils/utils.py` & `attr_utils-0.9.0/attr_utils/utils.py`

 * *Files identical despite different names*

### Comparing `attr_utils-0.8.1/attr_utils/autoattrs.py` & `attr_utils-0.9.0/attr_utils/autoattrs.py`

 * *Files 3% similar despite different names*

```diff
@@ -172,19 +172,31 @@
 			# TODO: work out what to do about this
 			warnings.simplefilter("ignore", RemovedInSphinx50Warning)
 			Documenter.add_content(self, more_content, True)
 
 		# set sourcename and add content from attribute documentation
 		sourcename = self.get_sourcename()
 
-		params, pre_output, post_output = self._get_docstring()
-
 		self.add_line('', sourcename)
-		for line in list(self.process_doc([pre_output])):
-			self.add_line(line, sourcename)
+
+		if hasattr(self.object, "__attrs_init__"):
+			# Size varies depending on docutils config
+			tab_size = self.env.app.config.docutils_tab_width
+
+			if self.object.__doc__:
+				docstring = dedent(self.object.__doc__).expandtabs(tab_size).split('\n')
+				for line in list(self.process_doc([docstring])):
+					self.add_line(line, sourcename)
+
+		else:
+			params, pre_output, post_output = self._get_docstring()
+
+			for line in list(self.process_doc([pre_output])):
+				self.add_line(line, sourcename)
+
 		self.add_line('', sourcename)
 
 	def _get_docstring(self) -> Tuple[Dict[str, Param], List[str], List[str]]:
 		"""
 		Returns params, pre_output, post_output.
 		"""
 
@@ -260,21 +272,22 @@
 			if not ''.join(doc).strip() and field in member_docstrings:
 				doc = member_docstrings[field]
 
 			field_entry = [f":param {field}:", *doc]
 			parameter_docs.append(' '.join(field_entry))
 			all_docs[field] = ''.join(doc).strip()
 
-		self.add_line('', sourcename)
+		if not hasattr(self.object, "__attrs_init__"):
+			self.add_line('', sourcename)
 
-		for line in self.process_doc([[*pre_output, *parameter_docs, '', '', *post_output]]):
-			if line and line in pre_output:
-				continue
-			self.add_line(line, sourcename)
-		self.add_line('', sourcename)
+			for line in self.process_doc([[*pre_output, *parameter_docs, '', '', *post_output]]):
+				if line and line in pre_output:
+					continue
+				self.add_line(line, sourcename)
+			self.add_line('', sourcename)
 
 		self._docstring_processed = True
 
 		if hasattr(self.object, "__slots__"):
 			slots_dict: MutableMapping[str, Optional[str]] = {}
 			for item in self.object.__slots__:  # type: ignore[attr-defined]
 				if item in all_docs:
```

