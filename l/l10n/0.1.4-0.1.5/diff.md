# Comparing `tmp/l10n-0.1.4.tar.gz` & `tmp/l10n-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "l10n-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "l10n-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `l10n-0.1.4.tar` & `l10n-0.1.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      710 2023-07-25 07:04:19.275434 l10n-0.1.4/.github/workflows/main.yml
--rw-r--r--   0        0        0       95 2023-03-31 11:41:21.762235 l10n-0.1.4/.gitignore
--rw-r--r--   0        0        0      325 2023-03-31 11:51:22.965953 l10n-0.1.4/.markdownlint.yaml
--rw-r--r--   0        0        0     1048 2023-03-31 07:51:09.539905 l10n-0.1.4/LICENSE
--rw-r--r--   0        0        0     3338 2023-03-31 11:51:52.001555 l10n-0.1.4/README.md
--rw-r--r--   0        0        0     3358 2023-03-31 11:41:21.762235 l10n-0.1.4/Taskfile.yml
--rw-r--r--   0        0        0     9237 2023-03-31 11:51:22.965953 l10n-0.1.4/docs/advanced.md
--rw-r--r--   0        0        0      110 2023-03-31 11:41:21.762235 l10n-0.1.4/docs/api.md
--rw-r--r--   0        0        0      317 2023-03-31 11:41:21.762235 l10n-0.1.4/docs/conf.py
--rw-r--r--   0        0        0      879 2023-03-31 11:51:02.630233 l10n-0.1.4/docs/index.md
--rw-r--r--   0        0        0     6540 2023-03-31 07:51:09.539905 l10n-0.1.4/docs/intro.md
--rw-r--r--   0        0        0     1070 2023-03-31 07:51:09.539905 l10n-0.1.4/docs/more.md
--rw-r--r--   0        0        0       77 2023-03-31 11:41:21.762235 l10n-0.1.4/docs/quickstart.md
--rw-r--r--   0        0        0     1355 2023-03-31 07:51:09.539905 l10n-0.1.4/docs/removed.md
--rw-r--r--   0        0        0       26 2023-03-31 07:51:09.539905 l10n-0.1.4/example-project/.gitignore
--rw-r--r--   0        0        0        0 2023-03-31 07:51:09.539905 l10n-0.1.4/example-project/example_project/__init__.py
--rw-r--r--   0        0        0       35 2023-03-31 11:41:21.762235 l10n-0.1.4/example-project/example_project/__main__.py
--rw-r--r--   0        0        0      461 2023-03-31 11:41:21.762235 l10n-0.1.4/example-project/example_project/example.py
--rw-r--r--   0        0        0      522 2023-03-31 07:51:09.539905 l10n-0.1.4/example-project/locales/en.po
--rw-r--r--   0        0        0      590 2023-03-31 07:51:09.539905 l10n-0.1.4/example-project/locales/ru.po
--rw-r--r--   0        0        0      262 2023-03-31 07:51:09.539905 l10n-0.1.4/example-project/pyproject.toml
--rw-r--r--   0        0        0      233 2023-07-25 09:51:11.292262 l10n-0.1.4/l10n/__init__.py
--rw-r--r--   0        0        0       44 2023-07-25 07:24:06.837236 l10n-0.1.4/l10n/__main__.py
--rw-r--r--   0        0        0      942 2023-07-25 07:24:06.837236 l10n-0.1.4/l10n/_cli.py
--rw-r--r--   0        0        0      335 2023-07-25 07:24:06.837236 l10n-0.1.4/l10n/_commands/__init__.py
--rw-r--r--   0        0        0      420 2023-07-25 07:24:06.837236 l10n-0.1.4/l10n/_commands/_base.py
--rw-r--r--   0        0        0     1920 2023-07-25 07:24:06.837236 l10n-0.1.4/l10n/_commands/_compile.py
--rw-r--r--   0        0        0     4867 2023-07-25 08:09:21.425920 l10n-0.1.4/l10n/_commands/_extract.py
--rw-r--r--   0        0        0     1943 2023-07-25 07:29:34.910563 l10n-0.1.4/l10n/_commands/_translate.py
--rw-r--r--   0        0        0     2824 2023-07-25 08:09:21.425920 l10n-0.1.4/l10n/_extractor.py
--rw-r--r--   0        0        0    12795 2023-07-25 07:24:06.837236 l10n-0.1.4/l10n/_locale.py
--rw-r--r--   0        0        0     3839 2023-07-25 07:24:06.837236 l10n-0.1.4/l10n/_locales.py
--rw-r--r--   0        0        0     3370 2023-07-25 07:24:06.837236 l10n-0.1.4/l10n/_plurals.py
--rw-r--r--   0        0        0     5170 2023-07-25 07:24:06.837236 l10n-0.1.4/l10n/_project.py
--rw-r--r--   0        0        0        0 2023-07-25 07:24:06.837236 l10n-0.1.4/l10n/py.typed
--rw-r--r--   0        0        0      693 2023-03-31 07:51:09.543905 l10n-0.1.4/messages.po
--rwxr-xr-x   0        0        0      128 2023-03-31 11:51:22.965953 l10n-0.1.4/netlify.sh
--rw-r--r--   0        0        0       95 2023-03-31 11:41:21.762235 l10n-0.1.4/netlify.toml
--rw-r--r--   0        0        0     2113 2023-07-25 09:50:28.851114 l10n-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       72 2023-03-31 11:41:21.762235 l10n-0.1.4/setup.cfg
--rw-r--r--   0        0        0        0 2023-03-31 07:51:09.543905 l10n-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0      468 2023-03-31 11:41:21.762235 l10n-0.1.4/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-03-31 07:51:09.543905 l10n-0.1.4/tests/test_commands/__init__.py
--rw-r--r--   0        0        0     1104 2023-03-31 11:41:21.762235 l10n-0.1.4/tests/test_commands/test_compile.py
--rw-r--r--   0        0        0     2724 2023-03-31 11:41:21.762235 l10n-0.1.4/tests/test_commands/test_extract.py
--rw-r--r--   0        0        0      854 2023-03-31 11:41:21.762235 l10n-0.1.4/tests/test_commands/test_translate.py
--rw-r--r--   0        0        0      309 2023-03-31 11:41:21.762235 l10n-0.1.4/tests/test_extractor.py
--rw-r--r--   0        0        0     6329 2023-03-31 11:41:21.762235 l10n-0.1.4/tests/test_locale.py
--rw-r--r--   0        0        0      708 2023-03-31 11:41:21.762235 l10n-0.1.4/tests/test_locales.py
--rw-r--r--   0        0        0     4913 1970-01-01 00:00:00.000000 l10n-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      710 2023-07-25 07:04:19.275434 l10n-0.1.5/.github/workflows/main.yml
+-rw-r--r--   0        0        0       95 2023-03-31 11:41:21.762235 l10n-0.1.5/.gitignore
+-rw-r--r--   0        0        0      325 2023-03-31 11:51:22.965953 l10n-0.1.5/.markdownlint.yaml
+-rw-r--r--   0        0        0     1048 2023-03-31 07:51:09.539905 l10n-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3338 2023-03-31 11:51:52.001555 l10n-0.1.5/README.md
+-rw-r--r--   0        0        0     3358 2023-03-31 11:41:21.762235 l10n-0.1.5/Taskfile.yml
+-rw-r--r--   0        0        0     9237 2023-03-31 11:51:22.965953 l10n-0.1.5/docs/advanced.md
+-rw-r--r--   0        0        0      110 2023-03-31 11:41:21.762235 l10n-0.1.5/docs/api.md
+-rw-r--r--   0        0        0      317 2023-03-31 11:41:21.762235 l10n-0.1.5/docs/conf.py
+-rw-r--r--   0        0        0      879 2023-03-31 11:51:02.630233 l10n-0.1.5/docs/index.md
+-rw-r--r--   0        0        0     6540 2023-03-31 07:51:09.539905 l10n-0.1.5/docs/intro.md
+-rw-r--r--   0        0        0     1070 2023-03-31 07:51:09.539905 l10n-0.1.5/docs/more.md
+-rw-r--r--   0        0        0       77 2023-03-31 11:41:21.762235 l10n-0.1.5/docs/quickstart.md
+-rw-r--r--   0        0        0     1355 2023-03-31 07:51:09.539905 l10n-0.1.5/docs/removed.md
+-rw-r--r--   0        0        0       26 2023-03-31 07:51:09.539905 l10n-0.1.5/example-project/.gitignore
+-rw-r--r--   0        0        0        0 2023-03-31 07:51:09.539905 l10n-0.1.5/example-project/example_project/__init__.py
+-rw-r--r--   0        0        0       35 2023-03-31 11:41:21.762235 l10n-0.1.5/example-project/example_project/__main__.py
+-rw-r--r--   0        0        0      461 2023-03-31 11:41:21.762235 l10n-0.1.5/example-project/example_project/example.py
+-rw-r--r--   0        0        0      522 2023-03-31 07:51:09.539905 l10n-0.1.5/example-project/locales/en.po
+-rw-r--r--   0        0        0      590 2023-03-31 07:51:09.539905 l10n-0.1.5/example-project/locales/ru.po
+-rw-r--r--   0        0        0      262 2023-03-31 07:51:09.539905 l10n-0.1.5/example-project/pyproject.toml
+-rw-r--r--   0        0        0      204 2023-07-31 08:37:37.269783 l10n-0.1.5/l10n/__init__.py
+-rw-r--r--   0        0        0       44 2023-07-25 07:24:06.837236 l10n-0.1.5/l10n/__main__.py
+-rw-r--r--   0        0        0      942 2023-07-25 07:24:06.837236 l10n-0.1.5/l10n/_cli.py
+-rw-r--r--   0        0        0      335 2023-07-25 07:24:06.837236 l10n-0.1.5/l10n/_commands/__init__.py
+-rw-r--r--   0        0        0      420 2023-07-25 07:24:06.837236 l10n-0.1.5/l10n/_commands/_base.py
+-rw-r--r--   0        0        0     1920 2023-07-25 07:24:06.837236 l10n-0.1.5/l10n/_commands/_compile.py
+-rw-r--r--   0        0        0     4867 2023-07-25 08:09:21.425920 l10n-0.1.5/l10n/_commands/_extract.py
+-rw-r--r--   0        0        0     1943 2023-07-25 07:29:34.910563 l10n-0.1.5/l10n/_commands/_translate.py
+-rw-r--r--   0        0        0     2824 2023-07-25 08:09:21.425920 l10n-0.1.5/l10n/_extractor.py
+-rw-r--r--   0        0        0    12795 2023-07-25 07:24:06.837236 l10n-0.1.5/l10n/_locale.py
+-rw-r--r--   0        0        0     3839 2023-07-25 07:24:06.837236 l10n-0.1.5/l10n/_locales.py
+-rw-r--r--   0        0        0     3370 2023-07-25 07:24:06.837236 l10n-0.1.5/l10n/_plurals.py
+-rw-r--r--   0        0        0     5170 2023-07-25 07:24:06.837236 l10n-0.1.5/l10n/_project.py
+-rw-r--r--   0        0        0        0 2023-07-25 07:24:06.837236 l10n-0.1.5/l10n/py.typed
+-rw-r--r--   0        0        0      693 2023-03-31 07:51:09.543905 l10n-0.1.5/messages.po
+-rwxr-xr-x   0        0        0      128 2023-03-31 11:51:22.965953 l10n-0.1.5/netlify.sh
+-rw-r--r--   0        0        0       95 2023-03-31 11:41:21.762235 l10n-0.1.5/netlify.toml
+-rw-r--r--   0        0        0     2118 2023-07-31 08:37:54.897685 l10n-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       72 2023-03-31 11:41:21.762235 l10n-0.1.5/setup.cfg
+-rw-r--r--   0        0        0        0 2023-03-31 07:51:09.543905 l10n-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0      468 2023-03-31 11:41:21.762235 l10n-0.1.5/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-03-31 07:51:09.543905 l10n-0.1.5/tests/test_commands/__init__.py
+-rw-r--r--   0        0        0     1104 2023-03-31 11:41:21.762235 l10n-0.1.5/tests/test_commands/test_compile.py
+-rw-r--r--   0        0        0     2724 2023-03-31 11:41:21.762235 l10n-0.1.5/tests/test_commands/test_extract.py
+-rw-r--r--   0        0        0      854 2023-03-31 11:41:21.762235 l10n-0.1.5/tests/test_commands/test_translate.py
+-rw-r--r--   0        0        0      309 2023-03-31 11:41:21.762235 l10n-0.1.5/tests/test_extractor.py
+-rw-r--r--   0        0        0     6329 2023-03-31 11:41:21.762235 l10n-0.1.5/tests/test_locale.py
+-rw-r--r--   0        0        0      708 2023-03-31 11:41:21.762235 l10n-0.1.5/tests/test_locales.py
+-rw-r--r--   0        0        0     4913 1970-01-01 00:00:00.000000 l10n-0.1.5/PKG-INFO
```

### Comparing `l10n-0.1.4/.github/workflows/main.yml` & `l10n-0.1.5/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/LICENSE` & `l10n-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/README.md` & `l10n-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/Taskfile.yml` & `l10n-0.1.5/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/docs/advanced.md` & `l10n-0.1.5/docs/advanced.md`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/docs/index.md` & `l10n-0.1.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/docs/intro.md` & `l10n-0.1.5/docs/intro.md`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/docs/more.md` & `l10n-0.1.5/docs/more.md`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/docs/removed.md` & `l10n-0.1.5/docs/removed.md`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/example-project/locales/en.po` & `l10n-0.1.5/example-project/locales/en.po`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/example-project/locales/ru.po` & `l10n-0.1.5/example-project/locales/ru.po`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/l10n/_cli.py` & `l10n-0.1.5/l10n/_cli.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/l10n/_commands/_compile.py` & `l10n-0.1.5/l10n/_commands/_compile.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/l10n/_commands/_extract.py` & `l10n-0.1.5/l10n/_commands/_extract.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/l10n/_commands/_translate.py` & `l10n-0.1.5/l10n/_commands/_translate.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/l10n/_extractor.py` & `l10n-0.1.5/l10n/_extractor.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/l10n/_locale.py` & `l10n-0.1.5/l10n/_locale.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/l10n/_locales.py` & `l10n-0.1.5/l10n/_locales.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/l10n/_plurals.py` & `l10n-0.1.5/l10n/_plurals.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/l10n/_project.py` & `l10n-0.1.5/l10n/_project.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/messages.po` & `l10n-0.1.5/messages.po`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/pyproject.toml` & `l10n-0.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 ]
 docs = ["sphinx", "myst-parser"]
 
 [project.urls]
 Source = "https://github.com/orsinium-labs/l10n"
 
 [project.scripts]
-l10n = "l10n:entrypoint"
+l10n = "l10n._cli:entrypoint"
 
 [tool.mypy]
 files = ["l10n", "tests"]
 python_version = 3.9
 ignore_missing_imports = true
 # follow_imports = "silent"
 show_error_codes = true
```

### Comparing `l10n-0.1.4/tests/test_commands/test_compile.py` & `l10n-0.1.5/tests/test_commands/test_compile.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/tests/test_commands/test_extract.py` & `l10n-0.1.5/tests/test_commands/test_extract.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/tests/test_commands/test_translate.py` & `l10n-0.1.5/tests/test_commands/test_translate.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/tests/test_locale.py` & `l10n-0.1.5/tests/test_locale.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/tests/test_locales.py` & `l10n-0.1.5/tests/test_locales.py`

 * *Files identical despite different names*

### Comparing `l10n-0.1.4/PKG-INFO` & `l10n-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: l10n
-Version: 0.1.4
+Version: 0.1.5
 Summary: A library and CLI for translating Python applications and libraries.
 Keywords: localization,internationalization,l10n,i18n,locale,locales,translation,gettext
 Author-email: Gram <gram@orsinium.dev>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

