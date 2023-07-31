# Comparing `tmp/python-lemming-0.6.1.tar.gz` & `tmp/python_lemming-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-lemming-0.6.1.tar", last modified: Thu Jul 20 10:39:31 2023, max compression
+gzip compressed data, was "python_lemming-0.6.2.tar", last modified: Mon Jul 31 19:01:58 2023, max compression
```

## Comparing `python-lemming-0.6.1.tar` & `python_lemming-0.6.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 10:39:31.964977 python-lemming-0.6.1/
--rw-rw-rw-   0        0        0    33094 2022-11-26 12:00:55.000000 python-lemming-0.6.1/LICENSE
--rw-rw-rw-   0        0        0    15930 2023-07-20 10:39:31.965977 python-lemming-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0    14865 2023-07-11 12:59:00.000000 python-lemming-0.6.1/README.md
--rw-rw-rw-   0        0        0     1615 2023-07-20 10:33:18.000000 python-lemming-0.6.1/pyproject.toml
--rw-rw-rw-   0        0        0     1557 2023-07-20 10:39:31.970978 python-lemming-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0       94 2022-12-17 14:25:46.000000 python-lemming-0.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 10:39:31.901430 python-lemming-0.6.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-20 10:39:31.926978 python-lemming-0.6.1/src/lemming/
--rw-rw-rw-   0        0        0      922 2023-07-20 10:37:18.000000 python-lemming-0.6.1/src/lemming/__init__.py
--rw-rw-rw-   0        0        0    17716 2023-07-20 10:31:15.000000 python-lemming-0.6.1/src/lemming/__main__.py
--rw-rw-rw-   0        0        0    13842 2023-07-11 12:59:00.000000 python-lemming-0.6.1/src/lemming/config.py
--rw-rw-rw-   0        0        0        0 2022-11-26 11:55:00.000000 python-lemming-0.6.1/src/lemming/py.typed
-drwxrwxrwx   0        0        0        0 2023-07-20 10:39:31.963977 python-lemming-0.6.1/src/python_lemming.egg-info/
--rw-rw-rw-   0        0        0    15930 2023-07-20 10:39:31.000000 python-lemming-0.6.1/src/python_lemming.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2023-07-20 10:39:31.000000 python-lemming-0.6.1/src/python_lemming.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 10:39:31.000000 python-lemming-0.6.1/src/python_lemming.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-07-20 10:39:31.000000 python-lemming-0.6.1/src/python_lemming.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-12-17 14:43:45.000000 python-lemming-0.6.1/src/python_lemming.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      113 2023-07-20 10:39:31.000000 python-lemming-0.6.1/src/python_lemming.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-20 10:39:31.000000 python-lemming-0.6.1/src/python_lemming.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 19:01:58.073050 python_lemming-0.6.2/
+-rw-rw-rw-   0        0        0    33094 2022-11-26 12:00:55.000000 python_lemming-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0    16094 2023-07-31 19:01:58.072050 python_lemming-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0    14865 2023-07-11 12:59:00.000000 python_lemming-0.6.2/README.md
+-rw-rw-rw-   0        0        0     3048 2023-07-31 18:59:28.000000 python_lemming-0.6.2/pyproject.toml
+-rw-rw-rw-   0        0        0      113 2023-07-11 11:26:23.000000 python_lemming-0.6.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 19:01:58.073621 python_lemming-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0       62 2023-07-31 18:56:12.000000 python_lemming-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 19:01:58.016451 python_lemming-0.6.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 19:01:58.035449 python_lemming-0.6.2/src/lemming/
+-rw-rw-rw-   0        0        0      922 2023-07-31 19:01:52.000000 python_lemming-0.6.2/src/lemming/__init__.py
+-rw-rw-rw-   0        0        0    17716 2023-07-20 10:31:15.000000 python_lemming-0.6.2/src/lemming/__main__.py
+-rw-rw-rw-   0        0        0    13842 2023-07-11 12:59:00.000000 python_lemming-0.6.2/src/lemming/config.py
+-rw-rw-rw-   0        0        0        0 2022-11-26 11:55:00.000000 python_lemming-0.6.2/src/lemming/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-31 19:01:58.070053 python_lemming-0.6.2/src/python_lemming.egg-info/
+-rw-rw-rw-   0        0        0    16094 2023-07-31 19:01:57.000000 python_lemming-0.6.2/src/python_lemming.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-07-31 19:01:57.000000 python_lemming-0.6.2/src/python_lemming.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 19:01:57.000000 python_lemming-0.6.2/src/python_lemming.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-31 19:01:57.000000 python_lemming-0.6.2/src/python_lemming.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      113 2023-07-31 19:01:57.000000 python_lemming-0.6.2/src/python_lemming.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-31 19:01:57.000000 python_lemming-0.6.2/src/python_lemming.egg-info/top_level.txt
```

### Comparing `python-lemming-0.6.1/LICENSE` & `python_lemming-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-lemming-0.6.1/PKG-INFO` & `python_lemming-0.6.2/src/python_lemming.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: python-lemming
-Version: 0.6.1
+Version: 0.6.2
 Summary: Lemming is a tool for formatting and linting code.
-Home-page: https://github.com/koviubi56/lemming
-Author: Koviubi56
-Author-email: koviubi56@duck.com
-License: GPL
+Author-email: Koviubi56 <koviubi56@duck.com>
+License: GPL-3.0-or-later
+Project-URL: Homepage, https://github.com/koviubi56/lemming
 Keywords: lemming,format,formatter,lint,linting,linter
-Platform: unix
-Platform: linux
-Platform: osx
-Platform: cygwin
-Platform: win32
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Lemming
 
 [![Hits-of-Code](https://hitsofcode.com/github/koviubi56/lemming?branch=main)](https://hitsofcode.com/github/koviubi56/lemming/view?branch=main)
```

### Comparing `python-lemming-0.6.1/README.md` & `python_lemming-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `python-lemming-0.6.1/src/lemming/__init__.py` & `python_lemming-0.6.2/src/lemming/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # SPDX-License-Identifier: GPL-3.0-or-later
 __all__ = ["__version__", "logger"]
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 import mylog
 
 logger = mylog.root.get_child("lemming")
 logger.threshold = mylog.Level.info
```

### Comparing `python-lemming-0.6.1/src/lemming/__main__.py` & `python_lemming-0.6.2/src/lemming/__main__.py`

 * *Files identical despite different names*

### Comparing `python-lemming-0.6.1/src/lemming/config.py` & `python_lemming-0.6.2/src/lemming/config.py`

 * *Files identical despite different names*

### Comparing `python-lemming-0.6.1/src/python_lemming.egg-info/PKG-INFO` & `python_lemming-0.6.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
-Name: python-lemming
-Version: 0.6.1
+Name: python_lemming
+Version: 0.6.2
 Summary: Lemming is a tool for formatting and linting code.
-Home-page: https://github.com/koviubi56/lemming
-Author: Koviubi56
-Author-email: koviubi56@duck.com
-License: GPL
+Author-email: Koviubi56 <koviubi56@duck.com>
+License: GPL-3.0-or-later
+Project-URL: Homepage, https://github.com/koviubi56/lemming
 Keywords: lemming,format,formatter,lint,linting,linter
-Platform: unix
-Platform: linux
-Platform: osx
-Platform: cygwin
-Platform: win32
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Lemming
 
 [![Hits-of-Code](https://hitsofcode.com/github/koviubi56/lemming?branch=main)](https://hitsofcode.com/github/koviubi56/lemming/view?branch=main)
```

