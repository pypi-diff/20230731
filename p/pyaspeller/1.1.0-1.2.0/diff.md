# Comparing `tmp/pyaspeller-1.1.0.tar.gz` & `tmp/pyaspeller-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaspeller-1.1.0.tar", max compression
+gzip compressed data, was "pyaspeller-1.2.0.tar", max compression
```

## Comparing `pyaspeller-1.1.0.tar` & `pyaspeller-1.2.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0    11338 2023-02-07 12:21:56.646675 pyaspeller-1.1.0/LICENSE
--rw-r--r--   0        0        0     1645 2023-02-07 12:21:56.646675 pyaspeller-1.1.0/README.md
--rw-r--r--   0        0        0     2164 2023-02-07 12:21:56.650675 pyaspeller-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4463 2023-02-07 12:21:56.650675 pyaspeller-1.1.0/src/pyaspeller/__init__.py
--rw-r--r--   0        0        0      207 2023-02-07 12:21:56.650675 pyaspeller-1.1.0/src/pyaspeller/errors.py
--rw-r--r--   0        0        0     4186 2023-02-07 12:21:56.650675 pyaspeller-1.1.0/src/pyaspeller/speller.py
--rw-r--r--   0        0        0     1320 2023-02-07 12:21:56.650675 pyaspeller-1.1.0/src/pyaspeller/word.py
--rw-r--r--   0        0        0     8205 2023-02-07 12:21:56.650675 pyaspeller-1.1.0/src/pyaspeller/yandex_speller.py
--rw-r--r--   0        0        0     2582 1970-01-01 00:00:00.000000 pyaspeller-1.1.0/setup.py
--rw-r--r--   0        0        0     2882 1970-01-01 00:00:00.000000 pyaspeller-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11338 2023-07-31 07:44:26.389902 pyaspeller-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1646 2023-07-31 07:44:26.389902 pyaspeller-1.2.0/README.md
+-rw-r--r--   0        0        0     2046 2023-07-31 07:44:26.389902 pyaspeller-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4844 2023-07-31 07:44:26.389902 pyaspeller-1.2.0/src/pyaspeller/__init__.py
+-rw-r--r--   0        0        0      325 2023-07-31 07:44:26.389902 pyaspeller-1.2.0/src/pyaspeller/errors.py
+-rw-r--r--   0        0        0     4606 2023-07-31 07:44:26.389902 pyaspeller-1.2.0/src/pyaspeller/speller.py
+-rw-r--r--   0        0        0     1393 2023-07-31 07:44:26.389902 pyaspeller-1.2.0/src/pyaspeller/word.py
+-rw-r--r--   0        0        0     9004 2023-07-31 07:44:26.389902 pyaspeller-1.2.0/src/pyaspeller/yandex_speller.py
+-rw-r--r--   0        0        0     2843 1970-01-01 00:00:00.000000 pyaspeller-1.2.0/PKG-INFO
```

### Comparing `pyaspeller-1.1.0/LICENSE` & `pyaspeller-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaspeller-1.1.0/README.md` & `pyaspeller-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -51,8 +51,8 @@
 
 Use your favourite package manager:
 
 ```bash
 $ python3 -m pip install pyaspeller
 ```
 
-Also there are available [rust](https://github.com/oriontvv/ryaspeller/) and [javascript](https://github.com/hcodes/yaspeller) versions of this speller.
+Also, there are available [rust](https://github.com/oriontvv/ryaspeller/) and [javascript](https://github.com/hcodes/yaspeller) versions of this speller.
```

### Comparing `pyaspeller-1.1.0/pyproject.toml` & `pyaspeller-1.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "pyaspeller"
-version = "1.1.0"
+version = "1.2.0"
 description = "Search tool typos in the text, files and websites."
 authors = [
-    "Vassiliy Taranov <taranov.vv@gmail.com>",
+    "Vasiliy Taranov <taranov.vv@gmail.com>",
 ]
 license = "Apache 2"
 readme = "README.md"
 homepage = "https://github.com/oriontvv/pyaspeller"
 repository = "https://github.com/oriontvv/pyaspeller"
 documentation = "https://github.com/oriontvv/pyaspeller"
 keywords = [
@@ -15,15 +15,15 @@
     "spelling",
     "spellcheck",
     "api",
     "yandex",
     "text",
 ]
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
     "Programming Language :: Python :: 3",
     "Topic :: Text Processing :: Linguistic"
 ]
@@ -31,81 +31,73 @@
     { include = "pyaspeller", from = "src" }
 ]
 
 [tool.poetry.scripts]
 pyaspeller = "src.pyaspeller.__init__:main"
 
 [tool.poetry.dependencies]
-python = "^3.6.2"
+python = "^3.7"
 requests = "^2.27.1"
 
 [tool.poetry.dev-dependencies]
-black = "^22.8.0"
 coveralls = { version = "^3.3.1", extras = [ "toml" ]}
-flake8 = "^5.0.4"
-isort = "^5.10.1"
 mypy = "^0.971"
 pytest = "^7.0.1"
 pytest-cov = "^4.0.0"
 pytest-deadfixtures = "^2.2.1"
-requests-mock = "^1.10.0"
+requests-mock = "^1.11.0"
 
 
+[tool.poetry.group.dev.dependencies]
+ruff = "^0.0.277"
+
 [build-system]
 requires = [
     "poetry>=0.12",
 ]
 build-backend = "poetry.masonry.api"
 
-[tool.flake8]
-ignore = [
-    "N801",
-    "N802",
-    "N803",
-    "E226",
-]
-max-complexity = 10
-
-[tool.pytest]
-addopts = "--ignore=py3 --ignore=build"
-
-
-[tool.black]
-line-length = 120
-exclude = '''
-/(
-    \.git
-  | \.hg
-  | \.mypy_cache
-  | \.tox
-  | \.venv
-  | _build
-  | buck-out
-  | build
-  | dist
-  | migrations
-)/
-'''
-
-[tool.isort]
-# make it compatible with black
-profile = "black"
-# Make sure this matches `*.py` in .editorconfig
-ensure_newline_before_comments = true
-include_trailing_comma = true
-use_parentheses = true
-
-
 [tool.coverage.run]
 relative_files = true
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "def __repr__",
     "if self.debug:",
     "if settings.DEBUG",
     "raise AssertionError",
     "raise NotImplementedError",
     "if 0:",
     "if __name__ == .__main__.:",
 ]
+
+[tool.ruff]
+ignore = [
+    "ANN101",
+    "N801",
+    "N802",
+    "N803",
+]
+line-length = 120
+select = [
+    "ANN",
+    "E",
+    "ERA",
+    "F",
+    "N",
+    "Q",
+    "TID",
+    "W",
+]
+
+[tool.ruff.flake8-annotations]
+mypy-init-return = true
+
+[tool.ruff.flake8-quotes]
+inline-quotes = "double"
+
+[tool.ruff.flake8-tidy-imports]
+ban-relative-imports = "all"
+
+[tool.mypy]
+ignore_missing_imports = true
```

### Comparing `pyaspeller-1.1.0/src/pyaspeller/speller.py` & `pyaspeller-1.2.0/src/pyaspeller/speller.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 import os
 from typing import Iterable, Union
 from pathlib import Path
 
 import requests
 
-from .errors import BadArgumentError
+from pyaspeller.errors import BadArgumentError, EncodingError
 
 _subs = {
     "\r\n": "\n",  # Fix Windows
     "\r": "\n",  # Fix MacOS
     "\n+": "\n",  # Repeat line ends
 }
 
@@ -36,16 +36,21 @@
 def is_path(path: Union[str, Path]) -> bool:
     return os.path.exists(path)
 
 
 class Speller:
     """
     Base spell class. Implements spelling logic for files.
+
+    Parameters:
+        :: encoding: encoding to use for opening and saving files
     """
 
+    encoding: str | None = None
+
     def spell(self, text: str) -> Iterable[object]:
         """
         Runs spell checking for text or URI and yields suggestions for changes.
 
         >>> spelled = speller.spell("42 is a cool maagic namber")
         >>> for p in spelled: print(p)
         {'code': 1, 'pos': 12, 'row': 0, 'col': 12, 'len': 6,
@@ -133,17 +138,23 @@
     def _spell_text(self, text: str) -> list[dict]:
         raise NotImplementedError()
 
     def _apply_suggestion(self, text: str, changes: Iterable[dict]) -> str:
         raise NotImplementedError()
 
     def _spell_file(self, path: str, apply: bool) -> Iterable[dict]:
-        with open(path) as infile:
-            content = infile.read()
+        with open(path, encoding=self.encoding) as infile:
+            try:
+                content = infile.read()
+            except UnicodeDecodeError as e:
+                raise EncodingError(
+                    "Encoding of the source file differs from the one was set. Please check encoding."
+                ) from e
+
             changes = self._spell_text(content)
 
             if apply:
                 updated = self._apply_suggestion(content, changes)
-                with open(path, "w") as outfile:
+                with open(path, "w", encoding=self.encoding) as outfile:
                     outfile.write(updated)
             else:
                 yield from changes
```

### Comparing `pyaspeller-1.1.0/src/pyaspeller/word.py` & `pyaspeller-1.2.0/src/pyaspeller/word.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 Contains definitions of Word class
 """
 from __future__ import annotations
 import warnings
 
-from .errors import BadArgumentError
-from .yandex_speller import YandexSpeller
+from pyaspeller.errors import BadArgumentError
+from pyaspeller.yandex_speller import YandexSpeller
 
 
 class Word:
     """
     Class for spelling of single word.
     """
 
-    def __init__(self, *args, **kwargs):
-        warnings.warn("Class Word is deprecated. Use Speller().spelled(text) instead")
+    def __init__(self, *args, **kwargs) -> None:  # noqa: ANN002 ANN003
+        warnings.warn("Class Word is deprecated. Use YandexSpeller().spelled(text) instead")
         if "text" in kwargs:
             text = kwargs.pop("text")
         else:
             text = args[0]
 
         if len(text.split()) > 1:
             msg = "Bad argument. Multiple words were detected."
@@ -29,15 +29,15 @@
         self.text = text
         self._answer = None
 
     @property
     def answer(self) -> list[dict]:
         if self._answer is None:
             self._answer = self._spell_text(self.text)
-        return self._answer
+        return self._answer  # type: ignore
 
     @property
     def correct(self) -> bool:
         return not self.answer
 
     @property
     def variants(self) -> list[str] | None:
```

### Comparing `pyaspeller-1.1.0/src/pyaspeller/yandex_speller.py` & `pyaspeller-1.2.0/src/pyaspeller/yandex_speller.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,49 +5,49 @@
 import collections
 import logging
 from typing import Iterable
 from urllib.parse import urlencode
 
 import requests
 
-from .errors import BadArgumentError
-from .speller import Speller
+from pyaspeller.errors import BadArgumentError
+from pyaspeller.speller import Speller
 
 
 class YandexSpeller(Speller):
     """
     Yandex speller implementation.
     """
 
-    _supported_langs = {"en", "ru", "uk"}
+    _supported_langs = ["en", "ru", "uk"]
 
     def __init__(
         self,
-        format_text=None,
-        lang=None,
-        config_path=None,
-        dictionary=None,
-        report_type=None,
-        max_requests=2,
-        is_debug=False,
-        check_yo=False,
-        ignore_urls=False,
-        ignore_tags=False,
-        ignore_capitalization=False,
-        ignore_digits=False,
-        ignore_latin=False,
-        ignore_roman_numerals=False,
-        ignore_uppercase=False,
-        find_repeat_words=False,
-        flag_latin=False,
-        by_words=False,
-    ):
-
-        self._lang = None
-        self.lang = lang or self._supported_langs
+        format_text: str | None = None,
+        lang: str | list[str] | None = None,
+        config_path: str | None = None,
+        dictionary: dict | None = None,
+        report_type: str | None = None,
+        max_requests: int = 2,
+        is_debug: bool = False,
+        check_yo: bool = False,
+        ignore_urls: bool = False,
+        ignore_tags: bool = False,
+        ignore_capitalization: bool = False,
+        ignore_digits: bool = False,
+        ignore_latin: bool = False,
+        ignore_roman_numerals: bool = False,
+        ignore_uppercase: bool = False,
+        find_repeat_words: bool = False,
+        flag_latin: bool = False,
+        by_words: bool = False,
+        encoding: str | None = None,
+    ) -> None:
+        self._lang: list[str] = []
+        self.lang = lang or self._supported_langs  # type: ignore
 
         if format_text == "auto" or not format_text:
             self._format = "plain"
         else:
             self._format = format_text
         self._config_path = config_path or ""
         self._dictionary = dictionary or {}
@@ -64,211 +64,219 @@
         self._find_repeat_words = find_repeat_words
         self._flag_latin = flag_latin
         self._by_words = by_words
 
         self._max_requests = max_requests
         self._is_debug = is_debug
 
-        self._api_query = "https://speller.yandex.net/services/spellservice.json/checkText"
+        self._api_query = (
+            "https://speller.yandex.net/services/spellservice.json/checkText"
+        )
+        self.encoding = encoding
 
     @property
-    def format(self):
+    def format(self) -> str:
         """Get format"""
         return self._format
 
     @format.setter
-    def format(self, value):
+    def format(self, value: str) -> None:
         """Set format"""
         self._format = value
 
     @property
-    def lang(self):
+    def lang(self) -> list[str]:
         """Get lang"""
         return self._lang
 
     @lang.setter
-    def lang(self, language):
+    def lang(self, language: str | Iterable[str]) -> None:
         """Set lang"""
         if isinstance(language, str):
             self._lang = [language]
         elif isinstance(language, collections.abc.Iterable):
             self._lang = list(language)
 
         if any(lang not in self._supported_langs for lang in self._lang):
             raise BadArgumentError("Unsupported language")
 
     @property
-    def config_path(self):
+    def config_path(self) -> str:
         """Get config_path"""
         return self._config_path
 
     @config_path.setter
-    def config_path(self, value):
+    def config_path(self, value: str) -> None:
         """Set config_path"""
         self._config_path = value or ""
         if not isinstance(self._config_path, str):
             msg = f"config_path must be a string: {self._config_path}"
             raise BadArgumentError(msg)
 
     @property
-    def dictionary(self):
+    def dictionary(self) -> dict:
         """Get dictionary"""
         return self._dictionary
 
     @dictionary.setter
-    def dictionary(self, value):
+    def dictionary(self, value: dict) -> None:
         """Set dictionary"""
         self._dictionary = value or {}
         if not isinstance(self._dictionary, dict):
             msg = f"dictionary must be a dict: {self._dictionary}"
             raise BadArgumentError(msg)
 
     @property
-    def report_type(self):
+    def report_type(self) -> str:
         """Get report_type"""
         return self._report_type
 
     @report_type.setter
-    def report_type(self, value):
+    def report_type(self, value: str) -> None:
         """Set report_type"""
         self._report_type = value or "console"
 
     @property
-    def check_yo(self):
+    def check_yo(self) -> bool:
         """Get check_yo"""
         return self._check_yo
 
     @check_yo.setter
-    def check_yo(self, value):
+    def check_yo(self, value: bool) -> None:
         """Set check_yo"""
         self._check_yo = value
 
     @property
-    def ignore_urls(self):
+    def ignore_urls(self) -> bool:
         """Get ignore_urls"""
         return self._ignore_urls
 
     @ignore_urls.setter
-    def ignore_urls(self, value):
+    def ignore_urls(self, value: bool) -> None:
         """Set ignore_urls"""
         self._ignore_urls = value
 
     @property
-    def ignore_tags(self):
+    def ignore_tags(self) -> bool:
         """Get ignore_tags"""
         return self._ignore_tags
 
     @ignore_tags.setter
-    def ignore_tags(self, value):
+    def ignore_tags(self, value: bool) -> None:
         """Set ignore_tags"""
         self._ignore_tags = value
 
     @property
-    def ignore_capitalization(self):
+    def ignore_capitalization(self) -> bool:
         """Get ignore_capitalization"""
         return self._ignore_capitalization
 
     @ignore_capitalization.setter
-    def ignore_capitalization(self, value):
+    def ignore_capitalization(self, value: bool) -> None:
         """Set ignore_capitalization"""
         self._ignore_capitalization = value
 
     @property
-    def ignore_digits(self):
+    def ignore_digits(self) -> bool:
         """Get ignore_digits"""
         return self._ignore_digits
 
     @ignore_digits.setter
-    def ignore_digits(self, value):
+    def ignore_digits(self, value: bool) -> None:
         """Set ignore_digits"""
         self._ignore_digits = value
 
     @property
-    def ignore_latin(self):
+    def ignore_latin(self) -> bool:
         """Get ignore_latin"""
         return self._ignore_latin
 
     @ignore_latin.setter
-    def ignore_latin(self, value):
+    def ignore_latin(self, value: bool) -> None:
         """Set ignore_latin"""
         self._ignore_latin = value
 
     @property
-    def ignore_roman_numerals(self):
+    def ignore_roman_numerals(self) -> bool:
         """Get ignore_roman_numerals"""
         return self._ignore_roman_numerals
 
     @ignore_roman_numerals.setter
-    def ignore_roman_numerals(self, value):
+    def ignore_roman_numerals(self, value: bool) -> None:
         """Set ignore_roman_numerals"""
         self._ignore_roman_numerals = value
 
     @property
-    def ignore_uppercase(self):
+    def ignore_uppercase(self) -> bool:
         """Get ignore_uppercase"""
         return self._ignore_uppercase
 
     @ignore_uppercase.setter
-    def ignore_uppercase(self, value):
+    def ignore_uppercase(self, value: bool) -> None:
         """Set ignore_uppercase"""
         self._ignore_uppercase = value
 
     @property
-    def find_repeat_words(self):
+    def find_repeat_words(self) -> bool:
         """Get find_repeat_words"""
         return self._find_repeat_words
 
     @find_repeat_words.setter
-    def find_repeat_words(self, value):
+    def find_repeat_words(self, value: bool) -> None:
         """Set find_repeat_words"""
         self._find_repeat_words = value
 
     @property
-    def flag_latin(self):
+    def flag_latin(self) -> bool:
         """Get flag_latin"""
         return self._flag_latin
 
     @flag_latin.setter
-    def flag_latin(self, value):
+    def flag_latin(self, value: bool) -> None:
         """Set flag_latin"""
         self._flag_latin = value
 
     @property
-    def by_words(self):
+    def by_words(self) -> bool:
         """Get by_words"""
         return self._by_words
 
     @by_words.setter
-    def by_words(self, value):
+    def by_words(self, value: bool) -> None:
         """Set by_words"""
         self._by_words = value
 
     @property
-    def max_requests(self):
+    def max_requests(self) -> int:
         """Get max_requests"""
         return self._max_requests
 
     @max_requests.setter
-    def max_requests(self, value):
+    def max_requests(self, value: int) -> None:
         """Set max_requests"""
         self._max_requests = value
 
     @property
-    def is_debug(self):
+    def is_debug(self) -> bool:
         """Get is_debug"""
         return self._is_debug
 
     @is_debug.setter
-    def is_debug(self, value):
+    def is_debug(self, value: bool) -> None:
         """Set is_debug"""
         self._is_debug = value
 
     def _spell_text(self, text: str) -> list[dict]:
         lang = ",".join(self._lang)
-        data = {"text": text, "options": self.api_options, "lang": lang, "format": self.format}
+        data = {
+            "text": text,
+            "options": self.api_options,
+            "lang": lang,
+            "format": self.format,
+        }
         response = requests.post(url=self._api_query, data=data).json()
 
         args = urlencode(data)
         logging.debug("%s?%s", self._api_query, args)
         logging.debug("response: %s", response)
         return response
```

### Comparing `pyaspeller-1.1.0/setup.py` & `pyaspeller-1.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,87 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pyaspeller
+Version: 1.2.0
+Summary: Search tool typos in the text, files and websites.
+Home-page: https://github.com/oriontvv/pyaspeller
+License: Apache 2
+Keywords: spell,spelling,spellcheck,api,yandex,text
+Author: Vasiliy Taranov
+Author-email: taranov.vv@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Text Processing :: Linguistic
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Project-URL: Documentation, https://github.com/oriontvv/pyaspeller
+Project-URL: Repository, https://github.com/oriontvv/pyaspeller
+Description-Content-Type: text/markdown
+
+# Python text speller
+
+[![CI](https://github.com/oriontvv/pyaspeller/workflows/ci/badge.svg)](https://github.com/oriontvv/pyaspeller/actions)       [![Coverage Status](https://img.shields.io/coveralls/oriontvv/pyaspeller.svg)](https://coveralls.io/r/oriontvv/pyaspeller) [![Pypi](http://img.shields.io/pypi/v/pyaspeller.svg?style=flat)](https://pypi.org/project/pyaspeller)
+
+
+[pyaspeller](https://github.com/oriontvv/pyaspeller) (Python Yandex Speller) is a cli tool and pure python library for searching typos in texts, files and websites.
+
+Spell checking uses [Yandex.Speller API](https://tech.yandex.ru/speller/doc/dg/concepts/About-docpage/). ([restrictions](<https://yandex.ru/legal/speller_api/>))
+
+
+## Features
+
+* Command line tool
+
+You can correct your local files or web pages
+
+```bash 
+$ pyaspeller ./doc
+$ pyaspeller https://team-tricky.github.io
+$ pyaspeller "в суббботу утромъ"
+в субботу утром
+```
+
+* Library 
+
+Use speller for your code
+
+```python
+>>> from pyaspeller import YandexSpeller
+>>> speller = YandexSpeller()
+>>> fixed = speller.spelled('Triky Custle is a great puzzle game.')
+>>> fixed
+'Tricky Castle is a great puzzle game.'
+```
+
+You can use class `Word` for single word queries:
+
+```python
+>>> from pyaspeller import Word
+>>> check = Word('tesst')
+>>> check.correct
+False
+>>> check.variants
+[u'test']
+>>> check.spellsafe
+u'test'
+```
+
+
+## Installation
+
+Use your favourite package manager:
+
+```bash
+$ python3 -m pip install pyaspeller
+```
 
-package_dir = \
-{'': 'src'}
+Also, there are available [rust](https://github.com/oriontvv/ryaspeller/) and [javascript](https://github.com/hcodes/yaspeller) versions of this speller.
 
-packages = \
-['pyaspeller']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['requests>=2.27.1,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['pyaspeller = src.pyaspeller.__init__:main']}
-
-setup_kwargs = {
-    'name': 'pyaspeller',
-    'version': '1.1.0',
-    'description': 'Search tool typos in the text, files and websites.',
-    'long_description': '# Python text speller\n\n[![CI](https://github.com/oriontvv/pyaspeller/workflows/ci/badge.svg)](https://github.com/oriontvv/pyaspeller/actions)       [![Coverage Status](https://img.shields.io/coveralls/oriontvv/pyaspeller.svg)](https://coveralls.io/r/oriontvv/pyaspeller) [![Pypi](http://img.shields.io/pypi/v/pyaspeller.svg?style=flat)](https://pypi.org/project/pyaspeller)\n\n\n[pyaspeller](https://github.com/oriontvv/pyaspeller) (Python Yandex Speller) is a cli tool and pure python library for searching typos in texts, files and websites.\n\nSpell checking uses [Yandex.Speller API](https://tech.yandex.ru/speller/doc/dg/concepts/About-docpage/). ([restrictions](<https://yandex.ru/legal/speller_api/>))\n\n\n## Features\n\n* Command line tool\n\nYou can correct your local files or web pages\n\n```bash \n$ pyaspeller ./doc\n$ pyaspeller https://team-tricky.github.io\n$ pyaspeller "в суббботу утромъ"\nв субботу утром\n```\n\n* Library \n\nUse speller for your code\n\n```python\n>>> from pyaspeller import YandexSpeller\n>>> speller = YandexSpeller()\n>>> fixed = speller.spelled(\'Triky Custle is a great puzzle game.\')\n>>> fixed\n\'Tricky Castle is a great puzzle game.\'\n```\n\nYou can use class `Word` for single word queries:\n\n```python\n>>> from pyaspeller import Word\n>>> check = Word(\'tesst\')\n>>> check.correct\nFalse\n>>> check.variants\n[u\'test\']\n>>> check.spellsafe\nu\'test\'\n```\n\n\n## Installation\n\nUse your favourite package manager:\n\n```bash\n$ python3 -m pip install pyaspeller\n```\n\nAlso there are available [rust](https://github.com/oriontvv/ryaspeller/) and [javascript](https://github.com/hcodes/yaspeller) versions of this speller.\n',
-    'author': 'Vassiliy Taranov',
-    'author_email': 'taranov.vv@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/oriontvv/pyaspeller',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6.2,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
```

