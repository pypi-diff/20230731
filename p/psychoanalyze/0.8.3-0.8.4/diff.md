# Comparing `tmp/psychoanalyze-0.8.3.tar.gz` & `tmp/psychoanalyze-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychoanalyze-0.8.3.tar", max compression
+gzip compressed data, was "psychoanalyze-0.8.4.tar", max compression
```

## Comparing `psychoanalyze-0.8.3.tar` & `psychoanalyze-0.8.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    35149 2022-10-04 02:36:06.350931 psychoanalyze-0.8.3/LICENSE
--rw-r--r--   0        0        0     1274 2023-07-26 11:57:00.456909 psychoanalyze-0.8.3/README.md
--rw-r--r--   0        0        0     1357 2023-07-10 06:32:31.020291 psychoanalyze-0.8.3/psychoanalyze/__init__.py
--rw-r--r--   0        0        0      756 2023-07-10 06:35:55.935533 psychoanalyze-0.8.3/psychoanalyze/analysis/__init__.py
--rw-r--r--   0        0        0     1288 2023-07-10 06:35:48.275360 psychoanalyze-0.8.3/psychoanalyze/analysis/bayes.py
--rw-r--r--   0        0        0     1120 2023-07-10 06:35:38.831225 psychoanalyze-0.8.3/psychoanalyze/analysis/ecdf.py
--rw-r--r--   0        0        0     2302 2023-07-10 23:10:13.757714 psychoanalyze-0.8.3/psychoanalyze/analysis/strength_duration.py
--rw-r--r--   0        0        0     2373 2023-07-10 06:35:32.351775 psychoanalyze-0.8.3/psychoanalyze/analysis/weber.py
--rw-r--r--   0        0        0     1070 2023-07-10 06:31:40.686289 psychoanalyze-0.8.3/psychoanalyze/dashboard/__init__.py
--rw-r--r--   0        0        0    12468 2023-07-28 02:10:21.380217 psychoanalyze-0.8.3/psychoanalyze/dashboard/app.py
--rw-r--r--   0        0        0    10618 2023-07-11 07:34:32.872491 psychoanalyze-0.8.3/psychoanalyze/dashboard/assets/PsychoAnalyze.svg
--rw-r--r--   0        0        0    33510 2023-07-11 07:34:42.444787 psychoanalyze-0.8.3/psychoanalyze/dashboard/assets/PsychoAnalyze_350x350.png
--rw-r--r--   0        0        0     6575 2023-07-20 04:43:03.897369 psychoanalyze-0.8.3/psychoanalyze/dashboard/assets/favicon.ico
--rw-r--r--   0        0        0     6575 2023-07-20 04:41:06.090118 psychoanalyze-0.8.3/psychoanalyze/dashboard/assets/logo_bgwhite.png
--rw-r--r--   0        0        0     5350 2023-07-11 09:34:15.577086 psychoanalyze-0.8.3/psychoanalyze/dashboard/assets/logo_transparent_100x100.png
--rw-r--r--   0        0        0      551 2023-07-15 02:24:50.772266 psychoanalyze-0.8.3/psychoanalyze/dashboard/assets/styles.css
--rw-r--r--   0        0        0     8915 2023-07-28 07:02:51.460865 psychoanalyze-0.8.3/psychoanalyze/dashboard/components.py
--rw-r--r--   0        0        0     9143 2023-07-28 09:06:06.449424 psychoanalyze-0.8.3/psychoanalyze/dashboard/layout.py
--rw-r--r--   0        0        0     1153 2023-07-20 09:25:55.060489 psychoanalyze-0.8.3/psychoanalyze/data/__init__.py
--rw-r--r--   0        0        0     6031 2023-07-28 00:17:06.312544 psychoanalyze-0.8.3/psychoanalyze/data/blocks.py
--rw-r--r--   0        0        0     6787 2023-07-28 00:17:06.312544 psychoanalyze-0.8.3/psychoanalyze/data/points.py
--rw-r--r--   0        0        0     2868 2023-07-10 06:35:10.993442 psychoanalyze-0.8.3/psychoanalyze/data/sessions.py
--rw-r--r--   0        0        0      841 2023-07-10 06:35:04.783422 psychoanalyze-0.8.3/psychoanalyze/data/stimulus.py
--rw-r--r--   0        0        0     1678 2023-07-10 06:34:48.603492 psychoanalyze-0.8.3/psychoanalyze/data/subjects.py
--rw-r--r--   0        0        0     5225 2023-07-20 09:41:06.475106 psychoanalyze-0.8.3/psychoanalyze/data/trials.py
--rw-r--r--   0        0        0     3002 2023-07-16 02:29:21.297443 psychoanalyze-0.8.3/psychoanalyze/data/types.py
--rw-r--r--   0        0        0     1135 2023-07-28 02:10:21.380217 psychoanalyze-0.8.3/psychoanalyze/main.py
--rw-r--r--   0        0        0     1239 2023-07-21 04:57:55.937376 psychoanalyze-0.8.3/psychoanalyze/params.py
--rw-r--r--   0        0        0     2116 2023-07-21 02:42:52.381174 psychoanalyze-0.8.3/psychoanalyze/plot.py
--rw-r--r--   0        0        0     1518 2023-07-10 06:34:24.801696 psychoanalyze-0.8.3/psychoanalyze/sigmoids.py
--rw-r--r--   0        0        0     3213 2023-07-30 01:28:15.197464 psychoanalyze-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 psychoanalyze-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-10-04 02:36:06.350931 psychoanalyze-0.8.4/LICENSE
+-rw-r--r--   0        0        0     1251 2023-07-31 00:45:44.501916 psychoanalyze-0.8.4/README.md
+-rw-r--r--   0        0        0     1357 2023-07-10 06:32:31.020291 psychoanalyze-0.8.4/psychoanalyze/__init__.py
+-rw-r--r--   0        0        0      756 2023-07-10 06:35:55.935533 psychoanalyze-0.8.4/psychoanalyze/analysis/__init__.py
+-rw-r--r--   0        0        0     1288 2023-07-10 06:35:48.275360 psychoanalyze-0.8.4/psychoanalyze/analysis/bayes.py
+-rw-r--r--   0        0        0     1120 2023-07-10 06:35:38.831225 psychoanalyze-0.8.4/psychoanalyze/analysis/ecdf.py
+-rw-r--r--   0        0        0     2302 2023-07-10 23:10:13.757714 psychoanalyze-0.8.4/psychoanalyze/analysis/strength_duration.py
+-rw-r--r--   0        0        0     2373 2023-07-10 06:35:32.351775 psychoanalyze-0.8.4/psychoanalyze/analysis/weber.py
+-rw-r--r--   0        0        0     1070 2023-07-10 06:31:40.686289 psychoanalyze-0.8.4/psychoanalyze/dashboard/__init__.py
+-rw-r--r--   0        0        0    12468 2023-07-28 02:10:21.380217 psychoanalyze-0.8.4/psychoanalyze/dashboard/app.py
+-rw-r--r--   0        0        0    10618 2023-07-11 07:34:32.872491 psychoanalyze-0.8.4/psychoanalyze/dashboard/assets/PsychoAnalyze.svg
+-rw-r--r--   0        0        0    33510 2023-07-11 07:34:42.444787 psychoanalyze-0.8.4/psychoanalyze/dashboard/assets/PsychoAnalyze_350x350.png
+-rw-r--r--   0        0        0     6575 2023-07-20 04:43:03.897369 psychoanalyze-0.8.4/psychoanalyze/dashboard/assets/favicon.ico
+-rw-r--r--   0        0        0     6575 2023-07-20 04:41:06.090118 psychoanalyze-0.8.4/psychoanalyze/dashboard/assets/logo_bgwhite.png
+-rw-r--r--   0        0        0     5350 2023-07-11 09:34:15.577086 psychoanalyze-0.8.4/psychoanalyze/dashboard/assets/logo_transparent_100x100.png
+-rw-r--r--   0        0        0      551 2023-07-15 02:24:50.772266 psychoanalyze-0.8.4/psychoanalyze/dashboard/assets/styles.css
+-rw-r--r--   0        0        0     8915 2023-07-28 07:02:51.460865 psychoanalyze-0.8.4/psychoanalyze/dashboard/components.py
+-rw-r--r--   0        0        0     9048 2023-07-31 00:45:44.521916 psychoanalyze-0.8.4/psychoanalyze/dashboard/layout.py
+-rw-r--r--   0        0        0     1153 2023-07-20 09:25:55.060489 psychoanalyze-0.8.4/psychoanalyze/data/__init__.py
+-rw-r--r--   0        0        0     6031 2023-07-28 00:17:06.312544 psychoanalyze-0.8.4/psychoanalyze/data/blocks.py
+-rw-r--r--   0        0        0     6787 2023-07-28 00:17:06.312544 psychoanalyze-0.8.4/psychoanalyze/data/points.py
+-rw-r--r--   0        0        0     2868 2023-07-10 06:35:10.993442 psychoanalyze-0.8.4/psychoanalyze/data/sessions.py
+-rw-r--r--   0        0        0      841 2023-07-10 06:35:04.783422 psychoanalyze-0.8.4/psychoanalyze/data/stimulus.py
+-rw-r--r--   0        0        0     1678 2023-07-10 06:34:48.603492 psychoanalyze-0.8.4/psychoanalyze/data/subjects.py
+-rw-r--r--   0        0        0     5225 2023-07-20 09:41:06.475106 psychoanalyze-0.8.4/psychoanalyze/data/trials.py
+-rw-r--r--   0        0        0     3002 2023-07-16 02:29:21.297443 psychoanalyze-0.8.4/psychoanalyze/data/types.py
+-rw-r--r--   0        0        0     1135 2023-07-28 02:10:21.380217 psychoanalyze-0.8.4/psychoanalyze/main.py
+-rw-r--r--   0        0        0     1239 2023-07-21 04:57:55.937376 psychoanalyze-0.8.4/psychoanalyze/params.py
+-rw-r--r--   0        0        0     2116 2023-07-21 02:42:52.381174 psychoanalyze-0.8.4/psychoanalyze/plot.py
+-rw-r--r--   0        0        0     1518 2023-07-10 06:34:24.801696 psychoanalyze-0.8.4/psychoanalyze/sigmoids.py
+-rw-r--r--   0        0        0     3191 2023-07-31 00:46:01.292011 psychoanalyze-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     3165 1970-01-01 00:00:00.000000 psychoanalyze-0.8.4/PKG-INFO
```

### Comparing `psychoanalyze-0.8.3/LICENSE` & `psychoanalyze-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/README.md` & `psychoanalyze-0.8.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/psychoanalyze)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 [![Open in Remote - Containers](https://img.shields.io/static/v1?label=Remote%20-%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/psychoanalyze/psychoanalyze)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/psychoanalyze/psychoanalyze/main.svg)](https://results.pre-commit.ci/latest/github/psychoanalyze/psychoanalyze/main)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/psychoanalyze/psychoanalyze/main?labpath=docs%2Fnotebooks%2Ftutorial.ipynb)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/psychoanalyze/notebooks/HEAD?labpath=tutorial.ipynb)
 
 
 ## Dashboard
 See what `psychoanalyze` can do by [viewing our dashboard](https://psychoanalyze.io/).
 
 ## Install with Python
 ```console
```

### Comparing `psychoanalyze-0.8.3/psychoanalyze/__init__.py` & `psychoanalyze-0.8.4/psychoanalyze/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/analysis/__init__.py` & `psychoanalyze-0.8.4/psychoanalyze/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/analysis/bayes.py` & `psychoanalyze-0.8.4/psychoanalyze/analysis/bayes.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/analysis/ecdf.py` & `psychoanalyze-0.8.4/psychoanalyze/analysis/ecdf.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/analysis/strength_duration.py` & `psychoanalyze-0.8.4/psychoanalyze/analysis/strength_duration.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/analysis/weber.py` & `psychoanalyze-0.8.4/psychoanalyze/analysis/weber.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/dashboard/__init__.py` & `psychoanalyze-0.8.4/psychoanalyze/dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/dashboard/app.py` & `psychoanalyze-0.8.4/psychoanalyze/dashboard/app.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/dashboard/assets/PsychoAnalyze.svg` & `psychoanalyze-0.8.4/psychoanalyze/dashboard/assets/PsychoAnalyze.svg`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/dashboard/assets/PsychoAnalyze_350x350.png` & `psychoanalyze-0.8.4/psychoanalyze/dashboard/assets/PsychoAnalyze_350x350.png`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/dashboard/assets/favicon.ico` & `psychoanalyze-0.8.4/psychoanalyze/dashboard/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/dashboard/assets/logo_bgwhite.png` & `psychoanalyze-0.8.4/psychoanalyze/dashboard/assets/logo_bgwhite.png`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/dashboard/assets/logo_transparent_100x100.png` & `psychoanalyze-0.8.4/psychoanalyze/dashboard/assets/logo_transparent_100x100.png`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/dashboard/assets/styles.css` & `psychoanalyze-0.8.4/psychoanalyze/dashboard/assets/styles.css`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/dashboard/components.py` & `psychoanalyze-0.8.4/psychoanalyze/dashboard/components.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/dashboard/layout.py` & `psychoanalyze-0.8.4/psychoanalyze/dashboard/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,17 +193,15 @@
         dcc.Store(id="trials-store"),
         dbc.NavbarSimple(
             [
                 dbc.NavItem(
                     [
                         dbc.NavLink(
                             "Notebook",
-                            href=(
-                                """https://nb.psychoanalyze.io/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2Fpsychoanalyze%2Fpsychoanalyze&urlpath=lab%2Ftree%2Fpsychoanalyze%2Fdocs%2Fnotebooks%2Ftutorial.ipynb&branch=main"""
-                            ),
+                            href="https://nb.psychoanalyze.io/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2Fpsychoanalyze%2Fnotebooks&urlpath=lab%2Ftree%2Fnotebooks%2Ftutorial.ipynb&branch=main",
                         ),
                         html.I(className="bi bi-journal-code"),
                     ],
                     className="d-flex align-items-center mx-2",
                 ),
                 dbc.NavItem(
                     [
```

### Comparing `psychoanalyze-0.8.3/psychoanalyze/data/__init__.py` & `psychoanalyze-0.8.4/psychoanalyze/data/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/data/blocks.py` & `psychoanalyze-0.8.4/psychoanalyze/data/blocks.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/data/points.py` & `psychoanalyze-0.8.4/psychoanalyze/data/points.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/data/sessions.py` & `psychoanalyze-0.8.4/psychoanalyze/data/sessions.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/data/stimulus.py` & `psychoanalyze-0.8.4/psychoanalyze/data/stimulus.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/data/subjects.py` & `psychoanalyze-0.8.4/psychoanalyze/data/subjects.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/data/trials.py` & `psychoanalyze-0.8.4/psychoanalyze/data/trials.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/data/types.py` & `psychoanalyze-0.8.4/psychoanalyze/data/types.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/main.py` & `psychoanalyze-0.8.4/psychoanalyze/main.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/params.py` & `psychoanalyze-0.8.4/psychoanalyze/params.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/plot.py` & `psychoanalyze-0.8.4/psychoanalyze/plot.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/psychoanalyze/sigmoids.py` & `psychoanalyze-0.8.4/psychoanalyze/sigmoids.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.3/pyproject.toml` & `psychoanalyze-0.8.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psychoanalyze"
-version = "0.8.3"
+version = "0.8.4"
 description = "Interactive analysis and simulation of psychophysical data."
 authors = ["Ty Schlichenmeyer <t.schlic@wustl.edu>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://psychoanalyze.io"
 repository = "https://github.com/psychoanalyze/psychoanalyze"
 documentation = "https://docs.psychoanalyze.io"
@@ -28,45 +28,44 @@
 pandas = "^2.0.2"
 scipy = "^1.10.1"
 numpy = "^1.25.0"
 dash-bootstrap-components = "^1.4.1"
 statsmodels = "^0.14.0"
 dash-daq = "^0.5.0"
 dash = "^2.11.1"
-dbt-duckdb = "^1.5.2"
 scikit-learn = "^1.2.2"
 bambi = "^0.11.0"
 cmdstanpy = "^1.1.0"
-pandas-stubs = "^2.0.2.230605"
-pandera = { extras = ["mypy"], version = "^0.15.1" }
-hypothesis = "^6.79.0"
-datatest = "^0.11.1"
+pandera = "^0.15.1"
 gunicorn = "^20.1.0"
-mypy = "^1.4.1"
 click = "^8.1.3"
 typer = { extras = ["all"], version = "^0.9.0" }
 kaleido = "0.2.1"
 pyarrow = "^12.0.1"
-types-pytz = "^2023.3.0.0"
-types-setuptools = "^68.0.0.3"
 
 [tool.poetry.scripts]
 psychoanalyze = "psychoanalyze.main:app"
 
 [tool.poetry.group.dev.dependencies]
+pandera = { extras = ["mypy"], version = "^0.15.1" }
+mypy = "^1.4.1"
 ipykernel = "^6.24.0"
 ipywidgets = "^8.0.7"
 jupyter = "^1.0.0"
 pytest-mock = "^3.11.1"
 tuna = "^0.5.11"
 ruff = "^0.0.280"
 black = "^23.3.0"
 python-semantic-release = "^8.0.2"
-dbt-core = "^1.5.3"
 pytest = "^7.3.2"
+types-pytz = "^2023.3.0.0"
+types-setuptools = "^68.0.0.3"
+hypothesis = "^6.79.0"
+pandas-stubs = "^2.0.2.230605"
+datatest = "^0.11.1"
 
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.1.21"
```

### Comparing `psychoanalyze-0.8.3/PKG-INFO` & `psychoanalyze-0.8.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychoanalyze
-Version: 0.8.3
+Version: 0.8.4
 Summary: Interactive analysis and simulation of psychophysical data.
 Home-page: https://psychoanalyze.io
 License: GPL-3.0-or-later
 Keywords: psychophysics,neuroscience,psychology
 Author: Ty Schlichenmeyer
 Author-email: t.schlic@wustl.edu
 Requires-Python: >=3.9.0,<3.12.0
@@ -23,31 +23,24 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Dist: bambi (>=0.11.0,<0.12.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cmdstanpy (>=1.1.0,<2.0.0)
 Requires-Dist: dash (>=2.11.1,<3.0.0)
 Requires-Dist: dash-bootstrap-components (>=1.4.1,<2.0.0)
 Requires-Dist: dash-daq (>=0.5.0,<0.6.0)
-Requires-Dist: datatest (>=0.11.1,<0.12.0)
-Requires-Dist: dbt-duckdb (>=1.5.2,<2.0.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
-Requires-Dist: hypothesis (>=6.79.0,<7.0.0)
 Requires-Dist: kaleido (==0.2.1)
-Requires-Dist: mypy (>=1.4.1,<2.0.0)
 Requires-Dist: numpy (>=1.25.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
-Requires-Dist: pandas-stubs (>=2.0.2.230605,<3.0.0.0)
-Requires-Dist: pandera[mypy] (>=0.15.1,<0.16.0)
+Requires-Dist: pandera (>=0.15.1,<0.16.0)
 Requires-Dist: pyarrow (>=12.0.1,<13.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
-Requires-Dist: types-pytz (>=2023.3.0.0,<2024.0.0.0)
-Requires-Dist: types-setuptools (>=68.0.0.3,<69.0.0.0)
 Project-URL: Documentation, https://docs.psychoanalyze.io
 Project-URL: JupyterHub, https://nb.psychoanalyze.io
 Project-URL: Repository, https://github.com/psychoanalyze/psychoanalyze
 Description-Content-Type: text/markdown
 
 # PsychoAnalyze
 
@@ -55,15 +48,15 @@
 
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/psychoanalyze)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 [![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)
 [![Open in Remote - Containers](https://img.shields.io/static/v1?label=Remote%20-%20Containers&message=Open&color=blue&logo=visualstudiocode)](https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/psychoanalyze/psychoanalyze)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/psychoanalyze/psychoanalyze/main.svg)](https://results.pre-commit.ci/latest/github/psychoanalyze/psychoanalyze/main)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/psychoanalyze/psychoanalyze/main?labpath=docs%2Fnotebooks%2Ftutorial.ipynb)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/psychoanalyze/notebooks/HEAD?labpath=tutorial.ipynb)
 
 
 ## Dashboard
 See what `psychoanalyze` can do by [viewing our dashboard](https://psychoanalyze.io/).
 
 ## Install with Python
 ```console
```

