# Comparing `tmp/moranpycess-1.0.39.tar.gz` & `tmp/moranpycess-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/angry-moran-simulator/angry-moran-simulator/dist/tmp6ap6ct65/moranpycess-1.0.39.tar", last modified: Fri May 28 22:41:04 2021, max compression
+gzip compressed data, was "moranpycess-1.1.0.tar", last modified: Mon Jul 31 13:35:37 2023, max compression
```

## Comparing `moranpycess-1.0.39.tar` & `moranpycess-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 22:41:04.000000 moranpycess-1.0.39/
--rw-r--r--   0 runner    (1001) docker     (121)      519 2021-05-28 22:40:56.000000 moranpycess-1.0.39/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     3257 2021-05-28 22:40:56.000000 moranpycess-1.0.39/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     4067 2021-05-28 22:40:56.000000 moranpycess-1.0.39/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2021-05-28 22:40:56.000000 moranpycess-1.0.39/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      111 2021-05-28 22:40:56.000000 moranpycess-1.0.39/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      946 2021-05-28 22:41:04.000000 moranpycess-1.0.39/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2882 2021-05-28 22:40:56.000000 moranpycess-1.0.39/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 22:41:04.000000 moranpycess-1.0.39/moranpycess/
--rw-r--r--   0 runner    (1001) docker     (121)     1400 2021-05-28 22:40:56.000000 moranpycess-1.0.39/moranpycess/CustomExceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2766 2021-05-28 22:40:56.000000 moranpycess-1.0.39/moranpycess/Individual.py
--rw-r--r--   0 runner    (1001) docker     (121)    23203 2021-05-28 22:40:56.000000 moranpycess-1.0.39/moranpycess/MoranProcess.py
--rw-r--r--   0 runner    (1001) docker     (121)    23977 2021-05-28 22:40:56.000000 moranpycess-1.0.39/moranpycess/MoranProcess2D.py
--rw-r--r--   0 runner    (1001) docker     (121)    30953 2021-05-28 22:40:56.000000 moranpycess-1.0.39/moranpycess/MoranProcess3D.py
--rw-r--r--   0 runner    (1001) docker     (121)      726 2021-05-28 22:40:56.000000 moranpycess-1.0.39/moranpycess/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-28 22:41:04.000000 moranpycess-1.0.39/moranpycess.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      946 2021-05-28 22:41:04.000000 moranpycess-1.0.39/moranpycess.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      489 2021-05-28 22:41:04.000000 moranpycess-1.0.39/moranpycess.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-28 22:41:04.000000 moranpycess-1.0.39/moranpycess.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-28 22:41:03.000000 moranpycess-1.0.39/moranpycess.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-05-28 22:41:04.000000 moranpycess-1.0.39/moranpycess.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-05-28 22:41:04.000000 moranpycess-1.0.39/moranpycess.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       95 2021-05-28 22:40:56.000000 moranpycess-1.0.39/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      784 2021-05-28 22:41:04.000000 moranpycess-1.0.39/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-05-28 22:40:56.000000 moranpycess-1.0.39/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:35:37.658381 moranpycess-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-31 13:35:26.000000 moranpycess-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-31 13:35:26.000000 moranpycess-1.1.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 13:35:26.000000 moranpycess-1.1.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-31 13:35:26.000000 moranpycess-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-31 13:35:26.000000 moranpycess-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-31 13:35:26.000000 moranpycess-1.1.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-31 13:35:26.000000 moranpycess-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-31 13:35:26.000000 moranpycess-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 13:35:37.658381 moranpycess-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-07-31 13:35:26.000000 moranpycess-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:35:37.650381 moranpycess-1.1.0/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-31 13:35:26.000000 moranpycess-1.1.0/dist/.pypi.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:35:37.650381 moranpycess-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:35:26.000000 moranpycess-1.1.0/docs/.nojekyll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:35:37.650381 moranpycess-1.1.0/docs/_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:35:26.000000 moranpycess-1.1.0/docs/_build/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:35:37.650381 moranpycess-1.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:35:26.000000 moranpycess-1.1.0/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:35:37.650381 moranpycess-1.1.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:35:26.000000 moranpycess-1.1.0/docs/_templates/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:35:37.650381 moranpycess-1.1.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-31 13:35:26.000000 moranpycess-1.1.0/docs/api/internal-api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-31 13:35:26.000000 moranpycess-1.1.0/docs/api/users-api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-31 13:35:26.000000 moranpycess-1.1.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:35:37.654381 moranpycess-1.1.0/docs/general-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-31 13:35:26.000000 moranpycess-1.1.0/docs/general-info/background.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-31 13:35:26.000000 moranpycess-1.1.0/docs/general-info/citing-contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-31 13:35:26.000000 moranpycess-1.1.0/docs/general-info/example-results.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-31 13:35:26.000000 moranpycess-1.1.0/docs/general-info/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-31 13:35:26.000000 moranpycess-1.1.0/docs/general-info/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-07-31 13:35:26.000000 moranpycess-1.1.0/docs/general-info/walkthrough.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-31 13:35:26.000000 moranpycess-1.1.0/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-07-31 13:35:26.000000 moranpycess-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 13:35:26.000000 moranpycess-1.1.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-31 13:35:26.000000 moranpycess-1.1.0/entrypoint.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:35:37.654381 moranpycess-1.1.0/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   463139 2023-07-31 13:35:26.000000 moranpycess-1.1.0/images/figure.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34289 2023-07-31 13:35:26.000000 moranpycess-1.1.0/images/scheme.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    35782 2023-07-31 13:35:26.000000 moranpycess-1.1.0/images/supplementary_figure1a.png
+-rw-r--r--   0 runner    (1001) docker     (123)   199895 2023-07-31 13:35:26.000000 moranpycess-1.1.0/images/supplementary_figure1b.png
+-rw-r--r--   0 runner    (1001) docker     (123)   206489 2023-07-31 13:35:26.000000 moranpycess-1.1.0/images/supplementary_figure2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   605339 2023-07-31 13:35:26.000000 moranpycess-1.1.0/images/supplementary_figureA1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-31 13:35:26.000000 moranpycess-1.1.0/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:35:37.658381 moranpycess-1.1.0/moranpycess/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-31 13:35:26.000000 moranpycess-1.1.0/moranpycess/CustomExceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-31 13:35:26.000000 moranpycess-1.1.0/moranpycess/Individual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23686 2023-07-31 13:35:26.000000 moranpycess-1.1.0/moranpycess/MoranProcess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24465 2023-07-31 13:35:26.000000 moranpycess-1.1.0/moranpycess/MoranProcess2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32400 2023-07-31 13:35:26.000000 moranpycess-1.1.0/moranpycess/MoranProcess3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-31 13:35:26.000000 moranpycess-1.1.0/moranpycess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:35:37.658381 moranpycess-1.1.0/moranpycess.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 13:35:37.000000 moranpycess-1.1.0/moranpycess.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-31 13:35:37.000000 moranpycess-1.1.0/moranpycess.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 13:35:37.000000 moranpycess-1.1.0/moranpycess.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 13:35:37.000000 moranpycess-1.1.0/moranpycess.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-31 13:35:37.000000 moranpycess-1.1.0/moranpycess.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 13:35:37.000000 moranpycess-1.1.0/moranpycess.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-31 13:35:26.000000 moranpycess-1.1.0/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-07-31 13:35:26.000000 moranpycess-1.1.0/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-31 13:35:26.000000 moranpycess-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 13:35:37.658381 moranpycess-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 13:35:26.000000 moranpycess-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `moranpycess-1.0.39/LICENSE` & `moranpycess-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moranpycess-1.0.39/PKG-INFO` & `moranpycess-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: moranpycess
-Version: 1.0.39
+Version: 1.1.0
 Summary: Python framework for Moran Processes driven by game theory
-Home-page: https://github.com/AngryMaciek/angry-moran-simulator
-Author: Maciek Bak
-Author-email: wsciekly.maciek@gmail.com
+Author-email: Maciek Bak <wsciekly.maciek@gmail.com>
 License: MIT
-Platform: UNKNOWN
+Project-URL: homepage, https://angrymaciek.github.io/angry-moran-simulator/_build/html/index.html
+Project-URL: repository, https://github.com/AngryMaciek/angry-moran-simulator
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 The following package presents a general game-theoretical framework to carry out scientific simulations according to the Moran model. Registering distinct types of individuals together with specification of payoffs between them allows to replicate evolution of the population and observe growth dynamics.
 
 For more information please visit project's homepage!
-
```

### Comparing `moranpycess-1.0.39/README.md` & `moranpycess-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+[![Contribute with Gitpod](https://img.shields.io/badge/Contribute%20with-Gitpod-908a85?logo=gitpod)](https://gitpod.io/#https://github.com/AngryMaciek/angry-moran-simulator)
+[![pre-commit](https://img.shields.io/badge/pre--commit-+-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![build](https://github.com/AngryMaciek/angry-moran-simulator/workflows/build/badge.svg?branch=master)](https://github.com/AngryMaciek/angry-moran-simulator/actions?query=workflow%3Abuild)
 [![pytest](https://github.com/AngryMaciek/angry-moran-simulator/workflows/pytest/badge.svg?branch=master)](https://github.com/AngryMaciek/angry-moran-simulator/actions?query=workflow%3Apytest)
 [![codecov](https://codecov.io/gh/AngryMaciek/angry-moran-simulator/branch/master/graph/badge.svg?token=V9IFEOWN71)](https://codecov.io/gh/AngryMaciek/angry-moran-simulator)
 [![flake8](https://github.com/AngryMaciek/angry-moran-simulator/workflows/flake8/badge.svg?branch=master)](https://github.com/AngryMaciek/angry-moran-simulator/actions?query=workflow%3Aflake8)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![CodeFactor](https://www.codefactor.io/repository/github/angrymaciek/angry-moran-simulator/badge)](https://www.codefactor.io/repository/github/angrymaciek/angry-moran-simulator)
 [![publish](https://github.com/AngryMaciek/angry-moran-simulator/workflows/publish/badge.svg)](https://github.com/AngryMaciek/angry-moran-simulator/actions?query=workflow%3Apublish)
-[![PyPI](https://img.shields.io/badge/pypi-1.0.39-blue)](https://pypi.org/project/moranpycess/)
+[![PyPI](https://img.shields.io/badge/pypi-1.1.0-blue)](https://pypi.org/project/moranpycess/)
 [![conda](https://anaconda.org/angrymaciek/moranpycess/badges/version.svg?service=github)](https://anaconda.org/AngryMaciek/moranpycess)
-[![DockerHub](https://img.shields.io/badge/DockerHub-1.0.39-blue)](https://hub.docker.com/r/angrymaciek/moranpycess)
+[![DockerHub](https://img.shields.io/badge/DockerHub-1.1.0-blue)](https://hub.docker.com/r/angrymaciek/moranpycess)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/AngryMaciek/angry-moran-simulator/master?filepath=tests%2Fusecase.ipynb)
 [![GitHub issues](https://img.shields.io/github/issues/AngryMaciek/angry-moran-simulator)](https://github.com/AngryMaciek/angry-moran-simulator/issues)
+[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md)
 [![GitHub license](https://img.shields.io/github/license/AngryMaciek/angry-moran-simulator)](https://github.com/AngryMaciek/angry-moran-simulator/blob/master/LICENSE)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.02643/status.svg)](https://doi.org/10.21105/joss.02643)
 
 # Moran [Py]cess
 
 ![scheme.svg](images/scheme.svg)
```

### Comparing `moranpycess-1.0.39/moranpycess/CustomExceptions.py` & `moranpycess-1.1.0/moranpycess/CustomExceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""
+""".
+
 ##############################################################################
 #
 #   Custom Exceptions
 #
 #   AUTHOR: Maciej_Bak
 #   AFFILIATION: University_of_Basel
 #   AFFILIATION: Swiss_Institute_of_Bioinformatics
```

### Comparing `moranpycess-1.0.39/moranpycess/Individual.py` & `moranpycess-1.1.0/moranpycess/Individual.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""
+""".
+
 ##############################################################################
 #
 #   Implementation of the population individuals
 #
 #   AUTHOR: Maciej_Bak
 #   AFFILIATION: University_of_Basel
 #   AFFILIATION: Swiss_Institute_of_Bioinformatics
@@ -41,64 +42,64 @@
         self.AvgBirthPayoff = None
         self.AvgDeathPayoff = None
         self.BirthFitness = None
         self.DeathFitness = None
 
     @property
     def ID(self):
-        """Python getter"""
+        """Python getter."""
         return self._ID
 
     @ID.setter
     def ID(self, ID):
-        """Python setter"""
+        """Python setter."""
         self._ID = ID
 
     @property
     def label(self):
-        """Python getter"""
+        """Python getter."""
         return self._label
 
     @label.setter
     def label(self, label):
-        """Python setter"""
+        """Python setter."""
         self._label = label
 
     @property
     def BirthFitness(self):
-        """Python getter"""
+        """Python getter."""
         return self._BirthFitness
 
     @BirthFitness.setter
     def BirthFitness(self, BirthFitness):
-        """Python setter"""
+        """Python setter."""
         self._BirthFitness = BirthFitness
 
     @property
     def DeathFitness(self):
-        """Python getter"""
+        """Python getter."""
         return self._DeathFitness
 
     @DeathFitness.setter
     def DeathFitness(self, DeathFitness):
-        """Python setter"""
+        """Python setter."""
         self._DeathFitness = DeathFitness
 
     @property
     def AvgBirthPayoff(self):
-        """Python getter"""
+        """Python getter."""
         return self._AvgBirthPayoff
 
     @AvgBirthPayoff.setter
     def AvgBirthPayoff(self, AvgBirthPayoff):
-        """Python setter"""
+        """Python setter."""
         self._AvgBirthPayoff = AvgBirthPayoff
 
     @property
     def AvgDeathPayoff(self):
-        """Python getter"""
+        """Python getter."""
         return self._AvgDeathPayoff
 
     @AvgDeathPayoff.setter
     def AvgDeathPayoff(self, AvgDeathPayoff):
-        """Python setter"""
+        """Python setter."""
         self._AvgDeathPayoff = AvgDeathPayoff
```

### Comparing `moranpycess-1.0.39/moranpycess/MoranProcess.py` & `moranpycess-1.1.0/moranpycess/MoranProcess.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-"""
+""".
+
 ##############################################################################
 #
 #   Implementation of the population evolution
 #
 #   AUTHOR: Maciej_Bak
 #   AFFILIATION: University_of_Basel
 #   AFFILIATION: Swiss_Institute_of_Bioinformatics
 #   CONTACT: wsciekly.maciek@gmail.com
 #   CREATED: 20-07-2020
 #   LICENSE: MIT
 #
 ##############################################################################
 """
 
+import copy
+
 # imports
 import random
-import copy
+
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import matplotlib.pyplot as plt
-from Individual import Individual
-from CustomExceptions import IncorrectValueError
+
+from moranpycess.CustomExceptions import IncorrectValueError
+from moranpycess.Individual import Individual
 
 
 class MoranProcess:
     """General Moran Process with multiple types of individuals."""
 
     def __init__(
         self,
@@ -68,15 +72,14 @@
                 between types. Defaults to None.
 
         Raises:
             AssertionError: on invalid arguments.
             IncorrectValueError: on wrong values in the Transition Matrix.
 
         """
-
         # check if the argument lists length match
         try:
             assert len(size_list) == len(label_list)
         except AssertionError as e:
             e.args += ("Mismatch length of size and label lists",)
             raise
 
@@ -150,19 +153,20 @@
                     == TransitionMatrix.shape[1]
                     == len(label_list)
                 )
             except AssertionError as e:
                 e.args += ("Invalid Transition Matrix",)
                 raise
             # check if the values are correct
+            message = "Transition probabilities need to add up to 1.0."
             for v in np.sum(TransitionMatrix, axis=1):
                 if v != 1.0:
                     raise IncorrectValueError(
                         parameter="Transition Matrix",
-                        message="Transition probabilities need to add up to 1.0.",
+                        message=message,
                     )
         self.TransitionMatrix = copy.deepcopy(TransitionMatrix)
 
     @property
     def population(self):
         """Python getter."""
         return self._population
@@ -363,15 +367,15 @@
         Returns:
             Individual: an individual selected from the population.
 
         """
         return self.__roulette_wheel_selection(attr="DeathFitness")
 
     def __roulette_wheel_selection(self, attr):
-        """A simple implementation of fitness proportional selection.
+        """Select individual based on fitness (fitness-proportional).
 
         Returns:
             Individual: an individual selected from the population.
 
         """
         if attr == "BirthFitness":
             max_value = sum(ind.BirthFitness for ind in self.population)
@@ -396,93 +400,107 @@
         Args:
             generations (int): number of time steps.
 
         Returns:
             pd.DataFrame: table with simulation logs.
 
         """
-
         # prepare a dataframe to store the logs
         colnames = (
-            [l + "__size" for l in self.init_label_list]
-            + [l + "__AvgBirthPayoff" for l in self.init_label_list]
-            + [l + "__AvgDeathPayoff" for l in self.init_label_list]
-            + [l + "__BirthFitness" for l in self.init_label_list]
-            + [l + "__DeathFitness" for l in self.init_label_list]
+            [label + "__size" for label in self.init_label_list]
+            + [label + "__AvgBirthPayoff" for label in self.init_label_list]
+            + [label + "__AvgDeathPayoff" for label in self.init_label_list]
+            + [label + "__BirthFitness" for label in self.init_label_list]
+            + [label + "__DeathFitness" for label in self.init_label_list]
             + ["Entropy"]
         )
         log_df = pd.DataFrame(index=range(generations + 1), columns=colnames)
         log_df.index.name = "generation"
 
         # update the dataframe with features of the initial population
-        for l in range(len(self.init_label_list)):
-            label = self.init_label_list[l]
-            log_df.at[0, label + "__size"] = self.init_size_list[l]
-            log_df.at[0, label + "__AvgBirthPayoff"] = self.AvgBirthPayoffDict[label]
-            log_df.at[0, label + "__AvgDeathPayoff"] = self.AvgDeathPayoffDict[label]
-            log_df.at[0, label + "__BirthFitness"] = self.BirthFitnessDict[label]
-            log_df.at[0, label + "__DeathFitness"] = self.DeathFitnessDict[label]
+        for index in range(len(self.init_label_list)):
+            label = self.init_label_list[index]
+            log_df.at[0, label + "__size"] = self.init_size_list[index]
+            log_df.at[0, label + "__AvgBirthPayoff"] = self.AvgBirthPayoffDict[
+                label
+            ]
+            log_df.at[0, label + "__AvgDeathPayoff"] = self.AvgDeathPayoffDict[
+                label
+            ]
+            log_df.at[0, label + "__BirthFitness"] = self.BirthFitnessDict[
+                label
+            ]
+            log_df.at[0, label + "__DeathFitness"] = self.DeathFitnessDict[
+                label
+            ]
             log_df.at[0, "Entropy"] = self.Entropy
 
         for g in range(generations):
-
             # select one individual to multiply
             selectedBirth = self._roulette_wheel_selection_Birth()
             # create a copy
             new_individual = copy.deepcopy(selectedBirth)
             # select one individual to die
             selectedDeath = self._roulette_wheel_selection_Death()
             # add the new individual to the population
             self.population.append(new_individual)
             # remove the selected individual from the population
             self.population.remove(selectedDeath)
             # update the list with population info
-            self.curr_size_list[self.init_label_list.index(selectedBirth.label)] += 1
-            self.curr_size_list[self.init_label_list.index(selectedDeath.label)] -= 1
+            self.curr_size_list[
+                self.init_label_list.index(selectedBirth.label)
+            ] += 1
+            self.curr_size_list[
+                self.init_label_list.index(selectedDeath.label)
+            ] -= 1
 
             # perform transitions (if TransitionMatrix was specified)
             if self.TransitionMatrix is not None:
                 for ind in self.population:
                     row_index = self.init_label_list.index(ind.label)
                     new_label = np.random.choice(
                         a=self.init_label_list,
                         size=1,
                         p=self.TransitionMatrix[row_index,],
                     )[0]
                     old_label = ind.label
                     ind.label = new_label
                     # update the list with population info
-                    self.curr_size_list[self.init_label_list.index(new_label)] += 1
-                    self.curr_size_list[self.init_label_list.index(old_label)] -= 1
+                    self.curr_size_list[
+                        self.init_label_list.index(new_label)
+                    ] += 1
+                    self.curr_size_list[
+                        self.init_label_list.index(old_label)
+                    ] -= 1
 
             # after each birth-death cycle:
-            # re-evaluate the payoffs and fitnesses of all Individuals in the population
+            # re-evaluate the payoffs and fitnesses of all ind in the pop
             self._UpdateAvgBirthPayoffForAll()
             self._UpdateAvgDeathPayoffForAll()
             self._UpdateBirthFitnessForAll()
             self._UpdateDeathFitnessForAll()
             # re-evaluate the population Entropy
             self._UpdateEntropy()
 
             # update the log dataframe
-            for l in range(len(self.init_label_list)):
-                label = self.init_label_list[l]
-                log_df.at[g + 1, label + "__size"] = self.curr_size_list[l]
-                log_df.at[g + 1, label + "__AvgBirthPayoff"] = self.AvgBirthPayoffDict[
-                    label
-                ]
-                log_df.at[g + 1, label + "__AvgDeathPayoff"] = self.AvgDeathPayoffDict[
-                    label
-                ]
-                log_df.at[g + 1, label + "__BirthFitness"] = self.BirthFitnessDict[
-                    label
-                ]
-                log_df.at[g + 1, label + "__DeathFitness"] = self.DeathFitnessDict[
-                    label
-                ]
+            for index in range(len(self.init_label_list)):
+                label = self.init_label_list[index]
+                log_df.at[g + 1, label + "__size"] = self.curr_size_list[index]
+                log_df.at[
+                    g + 1, label + "__AvgBirthPayoff"
+                ] = self.AvgBirthPayoffDict[label]
+                log_df.at[
+                    g + 1, label + "__AvgDeathPayoff"
+                ] = self.AvgDeathPayoffDict[label]
+                log_df.at[
+                    g + 1, label + "__BirthFitness"
+                ] = self.BirthFitnessDict[label]
+                log_df.at[
+                    g + 1, label + "__DeathFitness"
+                ] = self.DeathFitnessDict[label]
                 log_df.at[g + 1, "Entropy"] = self.Entropy
 
         return log_df
 
     def _UpdateEntropy(self):
         """Calculate entropy of Individual types in the population."""
         self.Entropy = 0
@@ -501,15 +519,15 @@
         """
         plt.figure(figsize=(14, 6))
         ax = plt.gca()
         ax.tick_params(width=1)
         for axis in ["top", "bottom", "left", "right"]:
             ax.spines[axis].set_linewidth(1)
         cmap = plt.get_cmap("coolwarm")
-        columns = [l + "__size" for l in self.init_label_list]
+        columns = [label + "__size" for label in self.init_label_list]
         df_copy = df[columns].copy()
         df_copy.columns = self.init_label_list
         df_copy.plot(linewidth=1.5, ax=ax, cmap=cmap)
         population_size = len(self.population)
         ax.set_ylim([0, population_size])
         plt.xlabel("Generation", size=14)
         plt.ylabel("# Individuals", size=14)
@@ -527,15 +545,17 @@
         """
         plt.figure(figsize=(14, 6))
         ax = plt.gca()
         ax.tick_params(width=1)
         for axis in ["top", "bottom", "left", "right"]:
             ax.spines[axis].set_linewidth(1)
         cmap = plt.get_cmap("coolwarm")
-        columns = [l + "__AvgBirthPayoff" for l in self.init_label_list]
+        columns = [
+            label + "__AvgBirthPayoff" for label in self.init_label_list
+        ]
         df_copy = df[columns].copy()
         df_copy.columns = self.init_label_list
         df_copy.plot(linewidth=1.5, ax=ax, cmap=cmap)
         plt.xlabel("Generation", size=14)
         plt.ylabel("Average Birth Payoff", size=14)
         ax.tick_params(axis="both", which="major", labelsize=12)
         ax.legend(loc=4, fontsize=20)
@@ -551,15 +571,17 @@
         """
         plt.figure(figsize=(14, 6))
         ax = plt.gca()
         ax.tick_params(width=1)
         for axis in ["top", "bottom", "left", "right"]:
             ax.spines[axis].set_linewidth(1)
         cmap = plt.get_cmap("coolwarm")
-        columns = [l + "__AvgDeathPayoff" for l in self.init_label_list]
+        columns = [
+            label + "__AvgDeathPayoff" for label in self.init_label_list
+        ]
         df_copy = df[columns].copy()
         df_copy.columns = self.init_label_list
         df_copy.plot(linewidth=1.5, ax=ax, cmap=cmap)
         plt.xlabel("Generation", size=14)
         plt.ylabel("Average Death Payoff", size=14)
         ax.tick_params(axis="both", which="major", labelsize=12)
         ax.legend(loc=4, fontsize=20)
@@ -575,15 +597,15 @@
         """
         plt.figure(figsize=(14, 6))
         ax = plt.gca()
         ax.tick_params(width=1)
         for axis in ["top", "bottom", "left", "right"]:
             ax.spines[axis].set_linewidth(1)
         cmap = plt.get_cmap("coolwarm")
-        columns = [l + "__BirthFitness" for l in self.init_label_list]
+        columns = [label + "__BirthFitness" for label in self.init_label_list]
         df_copy = df[columns].copy()
         df_copy.columns = self.init_label_list
         df_copy.plot(linewidth=1.5, ax=ax, cmap=cmap)
         plt.xlabel("Generation", size=14)
         plt.ylabel("Birth Fitness", size=14)
         ax.tick_params(axis="both", which="major", labelsize=12)
         ax.legend(loc=4, fontsize=20)
@@ -599,15 +621,15 @@
         """
         plt.figure(figsize=(14, 6))
         ax = plt.gca()
         ax.tick_params(width=1)
         for axis in ["top", "bottom", "left", "right"]:
             ax.spines[axis].set_linewidth(1)
         cmap = plt.get_cmap("coolwarm")
-        columns = [l + "__DeathFitness" for l in self.init_label_list]
+        columns = [label + "__DeathFitness" for label in self.init_label_list]
         df_copy = df[columns].copy()
         df_copy.columns = self.init_label_list
         df_copy.plot(linewidth=1.5, ax=ax, cmap=cmap)
         plt.xlabel("Generation", size=14)
         plt.ylabel("Death Fitness", size=14)
         ax.tick_params(axis="both", which="major", labelsize=12)
         ax.legend(loc=4, fontsize=20)
@@ -622,13 +644,15 @@
 
         """
         plt.figure(figsize=(14, 6))
         ax = plt.gca()
         ax.tick_params(width=1)
         for axis in ["top", "bottom", "left", "right"]:
             ax.spines[axis].set_linewidth(1)
-        df["Entropy"].plot(color="black", linewidth=1.5, ax=ax, label="Entropy")
+        df["Entropy"].plot(
+            color="black", linewidth=1.5, ax=ax, label="Entropy"
+        )
         plt.xlabel("Generation", size=14)
         plt.ylabel("", size=14)
         ax.tick_params(axis="both", which="major", labelsize=12)
         ax.legend(loc=4, fontsize=20)
         plt.savefig(fname=path, dpi=300)
```

### Comparing `moranpycess-1.0.39/moranpycess/MoranProcess2D.py` & `moranpycess-1.1.0/moranpycess/MoranProcess2D.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-"""
+""".
+
 ##############################################################################
 #
 #   Implementation of the 2D population evolution
 #
 #   AUTHOR: Maciej_Bak
 #   AFFILIATION: University_of_Basel
 #   AFFILIATION: Swiss_Institute_of_Bioinformatics
 #   CONTACT: wsciekly.maciek@gmail.com
 #   CREATED: 13-08-2020
 #   LICENSE: MIT
 #
 ##############################################################################
 """
 
+import copy
+
 # imports
 import random
-import copy
+
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import matplotlib.pyplot as plt
-from Individual import Individual
-from CustomExceptions import IncorrectValueError
+
+from moranpycess.CustomExceptions import IncorrectValueError
+from moranpycess.Individual import Individual
 
 
 class MoranProcess2D:
     """2D Moran Process with multiple types of individuals."""
 
     def __init__(
         self,
@@ -64,15 +68,14 @@
             curr_grid (np.array): subpopulations' initial position in 2D.
 
         Raises:
             AssertionError: on invalid arguments.
             IncorrectValueError: on wrong values in the Transition Matrix.
 
         """
-
         # check if the argument lists length match
         try:
             assert len(size_list) == len(label_list)
         except AssertionError as e:
             e.args += ("Mismatch length of size and label lists",)
             raise
 
@@ -112,26 +115,30 @@
         # introduce a payoff weight for the fitness calculation
         self.w = 0.5
 
         # check if the grid argument is correct
         try:
             unique, counts = np.unique(grid, return_counts=True)
             grid_dict = dict(zip(unique, counts))
-            for l in unique:
-                assert l in self.init_label_list
+            for label in unique:
+                assert label in self.init_label_list
             for i in range(len(unique)):
-                assert self.init_size_list[i] == grid_dict[self.init_label_list[i]]
+                assert (
+                    self.init_size_list[i]
+                    == grid_dict[self.init_label_list[i]]
+                )
         except AssertionError as e:
             e.args += ("Invalid Population Grid",)
             raise
 
         # initialize a 2D array of Individuals
         ID_counter = 0
         self.population = np.empty(
-            (self.init_grid.shape[0], self.init_grid.shape[1]), dtype=Individual,
+            (self.init_grid.shape[0], self.init_grid.shape[1]),
+            dtype=Individual,
         )
         for x in range(self.init_grid.shape[0]):
             for y in range(self.init_grid.shape[1]):
                 self.population[x, y] = Individual(
                     ID=ID_counter, label=self.init_grid[x, y]
                 )
                 ID_counter += 1
@@ -158,19 +165,20 @@
                     == TransitionMatrix.shape[1]
                     == len(label_list)
                 )
             except AssertionError as e:
                 e.args += ("Invalid Transition Matrix",)
                 raise
             # check if the values are correct
+            message = "Transition probabilities need to add up to 1.0."
             for v in np.sum(TransitionMatrix, axis=1):
                 if v != 1.0:
                     raise IncorrectValueError(
                         parameter="Transition Matrix",
-                        message="Transition probabilities need to add up to 1.0.",
+                        message=message,
                     )
         self.TransitionMatrix = copy.deepcopy(TransitionMatrix)
 
     @property
     def population(self):
         """Python getter."""
         return self._population
@@ -284,22 +292,21 @@
         """Calculate Birth Payoff for a given Individual.
 
         Args:
             x (int): x-coordinate of the Individual.
             y (int): y-coordinate of the Individual.
 
         """
-
         this_label = self.population[x, y].label
         this_label_index = self._init_label_list.index(this_label)
 
         pop_nrows = self.population.shape[0]
         pop_ncols = self.population.shape[1]
 
-        # Select direct neighbours in the grid with periodical boundary conditions:
+        # Select neighbours in the grid w/ periodical boundary conditions:
         # upper left, upper middle, upper right
         # middle left, middle right
         # lower left, lower middle, lower right
         neighbours_labels = [
             self.population[(x - 1) % pop_nrows, (y - 1) % pop_ncols].label,
             self.population[(x - 1) % pop_nrows, y % pop_ncols].label,
             self.population[(x - 1) % pop_nrows, (y + 1) % pop_ncols].label,
@@ -324,22 +331,21 @@
         """Calculate Death Payoff for a given Individual.
 
         Args:
             x (int): x-coordinate of the Individual.
             y (int): y-coordinate of the Individual.
 
         """
-
         this_label = self.population[x, y].label
         this_label_index = self._init_label_list.index(this_label)
 
         pop_nrows = self.population.shape[0]
         pop_ncols = self.population.shape[1]
 
-        # Select direct neighbours in the grid with periodical boundary conditions:
+        # Select neighbours in the grid w/ periodical boundary conditions:
         # upper left, upper middle, upper right
         # middle left, middle right
         # lower left, lower middle, lower right
         neighbours_labels = [
             self.population[(x - 1) % pop_nrows, (y - 1) % pop_ncols].label,
             self.population[(x - 1) % pop_nrows, y % pop_ncols].label,
             self.population[(x - 1) % pop_nrows, (y + 1) % pop_ncols].label,
@@ -424,22 +430,30 @@
         Returns:
             tuple: (X, Y) - coordinates of the selected Individual.
 
         """
         pop_nrows = self.population.shape[0]
         pop_ncols = self.population.shape[1]
         neighbours_scores = [
-            self.population[(x - 1) % pop_nrows, (y - 1) % pop_ncols].DeathFitness,
+            self.population[
+                (x - 1) % pop_nrows, (y - 1) % pop_ncols
+            ].DeathFitness,
             self.population[(x - 1) % pop_nrows, y % pop_ncols].DeathFitness,
-            self.population[(x - 1) % pop_nrows, (y + 1) % pop_ncols].DeathFitness,
+            self.population[
+                (x - 1) % pop_nrows, (y + 1) % pop_ncols
+            ].DeathFitness,
             self.population[x % pop_nrows, (y - 1) % pop_ncols].DeathFitness,
             self.population[x % pop_nrows, (y + 1) % pop_ncols].DeathFitness,
-            self.population[(x + 1) % pop_nrows, (y - 1) % pop_ncols].DeathFitness,
+            self.population[
+                (x + 1) % pop_nrows, (y - 1) % pop_ncols
+            ].DeathFitness,
             self.population[(x + 1) % pop_nrows, y % pop_ncols].DeathFitness,
-            self.population[(x + 1) % pop_nrows, (y + 1) % pop_ncols].DeathFitness,
+            self.population[
+                (x + 1) % pop_nrows, (y + 1) % pop_ncols
+            ].DeathFitness,
         ]
         max_value = sum(neighbours_scores)
         pick = random.uniform(0, max_value)
         current = 0
         indices_list = [
             ((x - 1) % pop_nrows, (y - 1) % pop_ncols),
             ((x - 1) % pop_nrows, y),
@@ -468,39 +482,44 @@
             pd.DataFrame: table with simulation logs.
 
         """
         pop_nrows = self.population.shape[0]
         pop_ncols = self.population.shape[1]
 
         # prepare a dataframe to store the logs
-        colnames = [l + "__size" for l in self.init_label_list] + ["Entropy"]
+        colnames = [label + "__size" for label in self.init_label_list] + [
+            "Entropy"
+        ]
         log_df = pd.DataFrame(index=range(generations + 1), columns=colnames)
         log_df.index.name = "generation"
 
         # update the dataframe with features of the initial population
-        for l in range(len(self.init_label_list)):
-            label = self.init_label_list[l]
-            log_df.at[0, label + "__size"] = self.init_size_list[l]
+        for index in range(len(self.init_label_list)):
+            label = self.init_label_list[index]
+            log_df.at[0, label + "__size"] = self.init_size_list[index]
             log_df.at[0, "Entropy"] = self.Entropy
 
         for g in range(generations):
-
             # select one individual to multiply
             (x, y) = self._roulette_wheel_selection_Birth()
             selectedBirth = self.population[x, y]
             # create a copy
             new_individual = copy.deepcopy(selectedBirth)
             # select one individual to die
             (x, y) = self._roulette_wheel_selection_Death(x, y)
             selectedDeath = copy.deepcopy(self.population[x, y])
             # swap the individuals
             self.population[x, y] = new_individual
             # update the list with population info
-            self.curr_size_list[self.init_label_list.index(selectedBirth.label)] += 1
-            self.curr_size_list[self.init_label_list.index(selectedDeath.label)] -= 1
+            self.curr_size_list[
+                self.init_label_list.index(selectedBirth.label)
+            ] += 1
+            self.curr_size_list[
+                self.init_label_list.index(selectedDeath.label)
+            ] -= 1
 
             # perform transitions (if TransitionMatrix was specified)
             if self.TransitionMatrix is not None:
                 for x_ in range(pop_nrows):
                     for y_ in range(pop_ncols):
                         ind = self.population[x_, y_]
                         row_index = self.init_label_list.index(ind.label)
@@ -508,32 +527,36 @@
                             a=self.init_label_list,
                             size=1,
                             p=self.TransitionMatrix[row_index,],
                         )[0]
                         old_label = ind.label
                         ind.label = new_label
                         # update the list with population info
-                        self.curr_size_list[self.init_label_list.index(new_label)] += 1
-                        self.curr_size_list[self.init_label_list.index(old_label)] -= 1
+                        self.curr_size_list[
+                            self.init_label_list.index(new_label)
+                        ] += 1
+                        self.curr_size_list[
+                            self.init_label_list.index(old_label)
+                        ] -= 1
 
             # after each birth-death cycle:
 
-            # update scores for all individuals (if TransitionMatrix was specified)
+            # update scores for all individuals (if TransitionMatrix present)
             if self.TransitionMatrix is not None:
                 for x_ in range(self.population.shape[0]):
                     for y_ in range(self.population.shape[1]):
                         self._UpdateBirthPayoff(x_, y_)
                         self._UpdateDeathPayoff(x_, y_)
                         self._UpdateBirthFitness(x_, y_)
                         self._UpdateDeathFitness(x_, y_)
             # in other case:
             # re-evaluate the payoffs and fitnesses of only
             # the affected neigbours Individuals in the population
             else:
-                # re-evaluate the payoffs and fitnesses of the affected Individuals in the population
+                # re-evaluate payoffs & fitnesses of affected ind in the pop
                 indices_list = [
                     ((x - 1) % pop_nrows, (y - 1) % pop_ncols),
                     ((x - 1) % pop_nrows, y),
                     ((x - 1) % pop_nrows, (y + 1) % pop_ncols),
                     (x, (y - 1) % pop_ncols),
                     (x, y),
                     (x, (y + 1) % pop_ncols),
@@ -552,17 +575,17 @@
                 for y_ in range(self.curr_grid.shape[1]):
                     self.curr_grid[x_, y_] = self.population[x_, y_].label
 
             # re-evaluate the population Entropy
             self._UpdateEntropy()
 
             # update the log dataframe
-            for l in range(len(self.init_label_list)):
-                label = self.init_label_list[l]
-                log_df.at[g + 1, label + "__size"] = self.curr_size_list[l]
+            for index in range(len(self.init_label_list)):
+                label = self.init_label_list[index]
+                log_df.at[g + 1, label + "__size"] = self.curr_size_list[index]
                 log_df.at[g + 1, "Entropy"] = self.Entropy
 
         return log_df
 
     def PlotSize2D(self, df, path):
         """Plot the sub-populations' sizes after a simulation.
 
@@ -573,15 +596,15 @@
         """
         plt.figure(figsize=(14, 6))
         ax = plt.gca()
         ax.tick_params(width=1)
         for axis in ["top", "bottom", "left", "right"]:
             ax.spines[axis].set_linewidth(1)
         cmap = plt.get_cmap("coolwarm")
-        columns = [l + "__size" for l in self.init_label_list]
+        columns = [label + "__size" for label in self.init_label_list]
         df_copy = df[columns].copy()
         df_copy.columns = self.init_label_list
         df_copy.plot(linewidth=1.5, ax=ax, cmap=cmap)
         population_size = self.population.size
         ax.set_ylim([0, population_size])
         plt.xlabel("Generation", size=14)
         plt.ylabel("# Individuals", size=14)
@@ -598,15 +621,17 @@
 
         """
         plt.figure(figsize=(14, 6))
         ax = plt.gca()
         ax.tick_params(width=1)
         for axis in ["top", "bottom", "left", "right"]:
             ax.spines[axis].set_linewidth(1)
-        df["Entropy"].plot(color="black", linewidth=1.5, ax=ax, label="Entropy")
+        df["Entropy"].plot(
+            color="black", linewidth=1.5, ax=ax, label="Entropy"
+        )
         plt.xlabel("Generation", size=14)
         plt.ylabel("", size=14)
         ax.tick_params(axis="both", which="major", labelsize=12)
         ax.legend(loc=4, fontsize=20)
         plt.savefig(fname=path, dpi=300)
 
     def PlotPopulationSnapshot2D(self, path):
@@ -620,15 +645,17 @@
         ax = plt.gca()
         ax.tick_params(width=1)
         for axis in ["top", "bottom", "left", "right"]:
             ax.spines[axis].set_linewidth(1)
         plot_grid = self.curr_grid.copy()
         ticks_labels = []
         for label_index in range(len(self.init_label_list)):
-            plot_grid[plot_grid == self.init_label_list[label_index]] = label_index
+            plot_grid[
+                plot_grid == self.init_label_list[label_index]
+            ] = label_index
             ticks_labels.append(self.init_label_list[label_index])
         plot_grid = plot_grid.astype(float)
         cmap = plt.get_cmap(
             "coolwarm", np.max(plot_grid) - np.min(plot_grid) + 1
         )  # get discrete colormap
         mat = plt.matshow(
             plot_grid,
```

### Comparing `moranpycess-1.0.39/moranpycess/MoranProcess3D.py` & `moranpycess-1.1.0/moranpycess/MoranProcess3D.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,34 @@
-"""
+""".
+
 ##############################################################################
 #
 #   Implementation of the 3D population evolution
 #
 #   AUTHOR: Maciej_Bak
 #   AFFILIATION: University_of_Basel
 #   AFFILIATION: Swiss_Institute_of_Bioinformatics
 #   CONTACT: wsciekly.maciek@gmail.com
 #   CREATED: 15-08-2020
 #   LICENSE: MIT
 #
 ##############################################################################
 """
 
+import copy
+
 # imports
 import random
-import copy
+
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import matplotlib.pyplot as plt
-from Individual import Individual
-from CustomExceptions import IncorrectValueError
+
+from moranpycess.CustomExceptions import IncorrectValueError
+from moranpycess.Individual import Individual
 
 
 class MoranProcess3D:
     """3D Moran Process with multiple types of individuals."""
 
     def __init__(
         self,
@@ -64,15 +68,14 @@
             curr_grid (np.array): subpopulations' initial position in 3D.
 
         Raises:
             AssertionError: on invalid arguments.
             IncorrectValueError: on wrong values in the Transition Matrix.
 
         """
-
         # check if the argument lists length match
         try:
             assert len(size_list) == len(label_list)
         except AssertionError as e:
             e.args += ("Mismatch length of size and label lists",)
             raise
 
@@ -112,26 +115,33 @@
         # introduce a payoff weight for the fitness calculation
         self.w = 0.5
 
         # check if the grid argument is correct
         try:
             unique, counts = np.unique(grid, return_counts=True)
             grid_dict = dict(zip(unique, counts))
-            for l in unique:
-                assert l in self.init_label_list
+            for label in unique:
+                assert label in self.init_label_list
             for i in range(len(unique)):
-                assert self.init_size_list[i] == grid_dict[self.init_label_list[i]]
+                assert (
+                    self.init_size_list[i]
+                    == grid_dict[self.init_label_list[i]]
+                )
         except AssertionError as e:
             e.args += ("Invalid Population Grid",)
             raise
 
         # initialize a 3D array of Individuals
         ID_counter = 0
         self.population = np.empty(
-            (self.init_grid.shape[0], self.init_grid.shape[1], self.init_grid.shape[2]),
+            (
+                self.init_grid.shape[0],
+                self.init_grid.shape[1],
+                self.init_grid.shape[2],
+            ),
             dtype=Individual,
         )
         for x in range(self.init_grid.shape[0]):
             for y in range(self.init_grid.shape[1]):
                 for z in range(self.init_grid.shape[2]):
                     self.population[x, y, z] = Individual(
                         ID=ID_counter, label=self.init_grid[x, y, z]
@@ -161,19 +171,20 @@
                     == TransitionMatrix.shape[1]
                     == len(label_list)
                 )
             except AssertionError as e:
                 e.args += ("Invalid Transition Matrix",)
                 raise
             # check if the values are correct
+            message = "Transition probabilities need to add up to 1.0."
             for v in np.sum(TransitionMatrix, axis=1):
                 if v != 1.0:
                     raise IncorrectValueError(
                         parameter="Transition Matrix",
-                        message="Transition probabilities need to add up to 1.0.",
+                        message=message,
                     )
         self.TransitionMatrix = copy.deepcopy(TransitionMatrix)
 
     @property
     def population(self):
         """Python getter."""
         return self._population
@@ -288,50 +299,65 @@
 
         Args:
             x (int): x-coordinate of the Individual.
             y (int): y-coordinate of the Individual.
             z (int): z-coordinate of the Individual.
 
         """
-
         this_label = self.population[x, y, z].label
         this_label_index = self._init_label_list.index(this_label)
 
         pop_x = self.population.shape[0]
         pop_y = self.population.shape[1]
         pop_z = self.population.shape[2]
 
-        # Select direct neighbours in the grid with periodical boundary conditions:
+        # Select neighbours in the grid with periodical boundary conditions:
         neighbours_labels = [
-            self.population[(x - 1) % pop_x, (y - 1) % pop_y, (z - 1) % pop_z].label,
+            self.population[
+                (x - 1) % pop_x, (y - 1) % pop_y, (z - 1) % pop_z
+            ].label,
             self.population[(x - 1) % pop_x, (y - 1) % pop_y, z % pop_z].label,
-            self.population[(x - 1) % pop_x, (y - 1) % pop_y, (z + 1) % pop_z].label,
+            self.population[
+                (x - 1) % pop_x, (y - 1) % pop_y, (z + 1) % pop_z
+            ].label,
             self.population[(x - 1) % pop_x, y % pop_y, (z - 1) % pop_z].label,
             self.population[(x - 1) % pop_x, y % pop_y, z % pop_z].label,
             self.population[(x - 1) % pop_x, y % pop_y, (z + 1) % pop_z].label,
-            self.population[(x - 1) % pop_x, (y + 1) % pop_y, (z - 1) % pop_z].label,
+            self.population[
+                (x - 1) % pop_x, (y + 1) % pop_y, (z - 1) % pop_z
+            ].label,
             self.population[(x - 1) % pop_x, (y + 1) % pop_y, z % pop_z].label,
-            self.population[(x - 1) % pop_x, (y + 1) % pop_y, (z + 1) % pop_z].label,
+            self.population[
+                (x - 1) % pop_x, (y + 1) % pop_y, (z + 1) % pop_z
+            ].label,
             self.population[x % pop_x, (y - 1) % pop_y, (z - 1) % pop_z].label,
             self.population[x % pop_x, (y - 1) % pop_y, z % pop_z].label,
             self.population[x % pop_x, (y - 1) % pop_y, (z + 1) % pop_z].label,
             self.population[x % pop_x, y % pop_y, (z - 1) % pop_z].label,
             self.population[x % pop_x, y % pop_y, (z + 1) % pop_z].label,
             self.population[x % pop_x, (y + 1) % pop_y, (z - 1) % pop_z].label,
             self.population[x % pop_x, (y + 1) % pop_y, z % pop_z].label,
             self.population[x % pop_x, (y + 1) % pop_y, (z + 1) % pop_z].label,
-            self.population[(x + 1) % pop_x, (y - 1) % pop_y, (z - 1) % pop_z].label,
+            self.population[
+                (x + 1) % pop_x, (y - 1) % pop_y, (z - 1) % pop_z
+            ].label,
             self.population[(x + 1) % pop_x, (y - 1) % pop_y, z % pop_z].label,
-            self.population[(x + 1) % pop_x, (y - 1) % pop_y, (z + 1) % pop_z].label,
+            self.population[
+                (x + 1) % pop_x, (y - 1) % pop_y, (z + 1) % pop_z
+            ].label,
             self.population[(x + 1) % pop_x, y % pop_y, (z - 1) % pop_z].label,
             self.population[(x + 1) % pop_x, y % pop_y, z % pop_z].label,
             self.population[(x + 1) % pop_x, y % pop_y, (z + 1) % pop_z].label,
-            self.population[(x + 1) % pop_x, (y + 1) % pop_y, (z - 1) % pop_z].label,
+            self.population[
+                (x + 1) % pop_x, (y + 1) % pop_y, (z - 1) % pop_z
+            ].label,
             self.population[(x + 1) % pop_x, (y + 1) % pop_y, z % pop_z].label,
-            self.population[(x + 1) % pop_x, (y + 1) % pop_y, (z + 1) % pop_z].label,
+            self.population[
+                (x + 1) % pop_x, (y + 1) % pop_y, (z + 1) % pop_z
+            ].label,
         ]
 
         payoff = 0
         for neighbour_label in set(neighbours_labels):
             c = self._init_label_list.index(neighbour_label)
             payoff += (
                 neighbours_labels.count(neighbour_label)
@@ -345,50 +371,65 @@
 
         Args:
             x (int): x-coordinate of the Individual.
             y (int): y-coordinate of the Individual.
             z (int): z-coordinate of the Individual.
 
         """
-
         this_label = self.population[x, y, z].label
         this_label_index = self._init_label_list.index(this_label)
 
         pop_x = self.population.shape[0]
         pop_y = self.population.shape[1]
         pop_z = self.population.shape[2]
 
-        # Select direct neighbours in the grid with periodical boundary conditions:
+        # Select neighbours in the grid with periodical boundary conditions:
         neighbours_labels = [
-            self.population[(x - 1) % pop_x, (y - 1) % pop_y, (z - 1) % pop_z].label,
+            self.population[
+                (x - 1) % pop_x, (y - 1) % pop_y, (z - 1) % pop_z
+            ].label,
             self.population[(x - 1) % pop_x, (y - 1) % pop_y, z % pop_z].label,
-            self.population[(x - 1) % pop_x, (y - 1) % pop_y, (z + 1) % pop_z].label,
+            self.population[
+                (x - 1) % pop_x, (y - 1) % pop_y, (z + 1) % pop_z
+            ].label,
             self.population[(x - 1) % pop_x, y % pop_y, (z - 1) % pop_z].label,
             self.population[(x - 1) % pop_x, y % pop_y, z % pop_z].label,
             self.population[(x - 1) % pop_x, y % pop_y, (z + 1) % pop_z].label,
-            self.population[(x - 1) % pop_x, (y + 1) % pop_y, (z - 1) % pop_z].label,
+            self.population[
+                (x - 1) % pop_x, (y + 1) % pop_y, (z - 1) % pop_z
+            ].label,
             self.population[(x - 1) % pop_x, (y + 1) % pop_y, z % pop_z].label,
-            self.population[(x - 1) % pop_x, (y + 1) % pop_y, (z + 1) % pop_z].label,
+            self.population[
+                (x - 1) % pop_x, (y + 1) % pop_y, (z + 1) % pop_z
+            ].label,
             self.population[x % pop_x, (y - 1) % pop_y, (z - 1) % pop_z].label,
             self.population[x % pop_x, (y - 1) % pop_y, z % pop_z].label,
             self.population[x % pop_x, (y - 1) % pop_y, (z + 1) % pop_z].label,
             self.population[x % pop_x, y % pop_y, (z - 1) % pop_z].label,
             self.population[x % pop_x, y % pop_y, (z + 1) % pop_z].label,
             self.population[x % pop_x, (y + 1) % pop_y, (z - 1) % pop_z].label,
             self.population[x % pop_x, (y + 1) % pop_y, z % pop_z].label,
             self.population[x % pop_x, (y + 1) % pop_y, (z + 1) % pop_z].label,
-            self.population[(x + 1) % pop_x, (y - 1) % pop_y, (z - 1) % pop_z].label,
+            self.population[
+                (x + 1) % pop_x, (y - 1) % pop_y, (z - 1) % pop_z
+            ].label,
             self.population[(x + 1) % pop_x, (y - 1) % pop_y, z % pop_z].label,
-            self.population[(x + 1) % pop_x, (y - 1) % pop_y, (z + 1) % pop_z].label,
+            self.population[
+                (x + 1) % pop_x, (y - 1) % pop_y, (z + 1) % pop_z
+            ].label,
             self.population[(x + 1) % pop_x, y % pop_y, (z - 1) % pop_z].label,
             self.population[(x + 1) % pop_x, y % pop_y, z % pop_z].label,
             self.population[(x + 1) % pop_x, y % pop_y, (z + 1) % pop_z].label,
-            self.population[(x + 1) % pop_x, (y + 1) % pop_y, (z - 1) % pop_z].label,
+            self.population[
+                (x + 1) % pop_x, (y + 1) % pop_y, (z - 1) % pop_z
+            ].label,
             self.population[(x + 1) % pop_x, (y + 1) % pop_y, z % pop_z].label,
-            self.population[(x + 1) % pop_x, (y + 1) % pop_y, (z + 1) % pop_z].label,
+            self.population[
+                (x + 1) % pop_x, (y + 1) % pop_y, (z + 1) % pop_z
+            ].label,
         ]
 
         payoff = 0
         for neighbour_label in set(neighbours_labels):
             c = self._init_label_list.index(neighbour_label)
             payoff += (
                 neighbours_labels.count(neighbour_label)
@@ -470,50 +511,86 @@
         pop_x = self.population.shape[0]
         pop_y = self.population.shape[1]
         pop_z = self.population.shape[2]
         neighbours_scores = [
             self.population[
                 (x - 1) % pop_x, (y - 1) % pop_y, (z - 1) % pop_z
             ].DeathFitness,
-            self.population[(x - 1) % pop_x, (y - 1) % pop_y, z % pop_z].DeathFitness,
+            self.population[
+                (x - 1) % pop_x, (y - 1) % pop_y, z % pop_z
+            ].DeathFitness,
             self.population[
                 (x - 1) % pop_x, (y - 1) % pop_y, (z + 1) % pop_z
             ].DeathFitness,
-            self.population[(x - 1) % pop_x, y % pop_y, (z - 1) % pop_z].DeathFitness,
-            self.population[(x - 1) % pop_x, y % pop_y, z % pop_z].DeathFitness,
-            self.population[(x - 1) % pop_x, y % pop_y, (z + 1) % pop_z].DeathFitness,
+            self.population[
+                (x - 1) % pop_x, y % pop_y, (z - 1) % pop_z
+            ].DeathFitness,
+            self.population[
+                (x - 1) % pop_x, y % pop_y, z % pop_z
+            ].DeathFitness,
+            self.population[
+                (x - 1) % pop_x, y % pop_y, (z + 1) % pop_z
+            ].DeathFitness,
             self.population[
                 (x - 1) % pop_x, (y + 1) % pop_y, (z - 1) % pop_z
             ].DeathFitness,
-            self.population[(x - 1) % pop_x, (y + 1) % pop_y, z % pop_z].DeathFitness,
+            self.population[
+                (x - 1) % pop_x, (y + 1) % pop_y, z % pop_z
+            ].DeathFitness,
             self.population[
                 (x - 1) % pop_x, (y + 1) % pop_y, (z + 1) % pop_z
             ].DeathFitness,
-            self.population[x % pop_x, (y - 1) % pop_y, (z - 1) % pop_z].DeathFitness,
-            self.population[x % pop_x, (y - 1) % pop_y, z % pop_z].DeathFitness,
-            self.population[x % pop_x, (y - 1) % pop_y, (z + 1) % pop_z].DeathFitness,
-            self.population[x % pop_x, y % pop_y, (z - 1) % pop_z].DeathFitness,
-            self.population[x % pop_x, y % pop_y, (z + 1) % pop_z].DeathFitness,
-            self.population[x % pop_x, (y + 1) % pop_y, (z - 1) % pop_z].DeathFitness,
-            self.population[x % pop_x, (y + 1) % pop_y, z % pop_z].DeathFitness,
-            self.population[x % pop_x, (y + 1) % pop_y, (z + 1) % pop_z].DeathFitness,
+            self.population[
+                x % pop_x, (y - 1) % pop_y, (z - 1) % pop_z
+            ].DeathFitness,
+            self.population[
+                x % pop_x, (y - 1) % pop_y, z % pop_z
+            ].DeathFitness,
+            self.population[
+                x % pop_x, (y - 1) % pop_y, (z + 1) % pop_z
+            ].DeathFitness,
+            self.population[
+                x % pop_x, y % pop_y, (z - 1) % pop_z
+            ].DeathFitness,
+            self.population[
+                x % pop_x, y % pop_y, (z + 1) % pop_z
+            ].DeathFitness,
+            self.population[
+                x % pop_x, (y + 1) % pop_y, (z - 1) % pop_z
+            ].DeathFitness,
+            self.population[
+                x % pop_x, (y + 1) % pop_y, z % pop_z
+            ].DeathFitness,
+            self.population[
+                x % pop_x, (y + 1) % pop_y, (z + 1) % pop_z
+            ].DeathFitness,
             self.population[
                 (x + 1) % pop_x, (y - 1) % pop_y, (z - 1) % pop_z
             ].DeathFitness,
-            self.population[(x + 1) % pop_x, (y - 1) % pop_y, z % pop_z].DeathFitness,
+            self.population[
+                (x + 1) % pop_x, (y - 1) % pop_y, z % pop_z
+            ].DeathFitness,
             self.population[
                 (x + 1) % pop_x, (y - 1) % pop_y, (z + 1) % pop_z
             ].DeathFitness,
-            self.population[(x + 1) % pop_x, y % pop_y, (z - 1) % pop_z].DeathFitness,
-            self.population[(x + 1) % pop_x, y % pop_y, z % pop_z].DeathFitness,
-            self.population[(x + 1) % pop_x, y % pop_y, (z + 1) % pop_z].DeathFitness,
+            self.population[
+                (x + 1) % pop_x, y % pop_y, (z - 1) % pop_z
+            ].DeathFitness,
+            self.population[
+                (x + 1) % pop_x, y % pop_y, z % pop_z
+            ].DeathFitness,
+            self.population[
+                (x + 1) % pop_x, y % pop_y, (z + 1) % pop_z
+            ].DeathFitness,
             self.population[
                 (x + 1) % pop_x, (y + 1) % pop_y, (z - 1) % pop_z
             ].DeathFitness,
-            self.population[(x + 1) % pop_x, (y + 1) % pop_y, z % pop_z].DeathFitness,
+            self.population[
+                (x + 1) % pop_x, (y + 1) % pop_y, z % pop_z
+            ].DeathFitness,
             self.population[
                 (x + 1) % pop_x, (y + 1) % pop_y, (z + 1) % pop_z
             ].DeathFitness,
         ]
         max_value = sum(neighbours_scores)
         pick = random.uniform(0, max_value)
         current = 0
@@ -564,39 +641,44 @@
 
         """
         pop_x = self.population.shape[0]
         pop_y = self.population.shape[1]
         pop_z = self.population.shape[2]
 
         # prepare a dataframe to store the logs
-        colnames = [l + "__size" for l in self.init_label_list] + ["Entropy"]
+        colnames = [label + "__size" for label in self.init_label_list] + [
+            "Entropy"
+        ]
         log_df = pd.DataFrame(index=range(generations + 1), columns=colnames)
         log_df.index.name = "generation"
 
         # update the dataframe with features of the initial population
-        for l in range(len(self.init_label_list)):
-            label = self.init_label_list[l]
-            log_df.at[0, label + "__size"] = self.init_size_list[l]
+        for index in range(len(self.init_label_list)):
+            label = self.init_label_list[index]
+            log_df.at[0, label + "__size"] = self.init_size_list[index]
             log_df.at[0, "Entropy"] = self.Entropy
 
         for g in range(generations):
-
             # select one individual to multiply
             (x, y, z) = self._roulette_wheel_selection_Birth()
             selectedBirth = self.population[x, y, z]
             # create a copy
             new_individual = copy.deepcopy(selectedBirth)
             # select one individual to die
             (x, y, z) = self._roulette_wheel_selection_Death(x, y, z)
             selectedDeath = copy.deepcopy(self.population[x, y, z])
             # swap the individuals
             self.population[x, y, z] = new_individual
             # update the list with population info
-            self.curr_size_list[self.init_label_list.index(selectedBirth.label)] += 1
-            self.curr_size_list[self.init_label_list.index(selectedDeath.label)] -= 1
+            self.curr_size_list[
+                self.init_label_list.index(selectedBirth.label)
+            ] += 1
+            self.curr_size_list[
+                self.init_label_list.index(selectedDeath.label)
+            ] -= 1
 
             # perform transitions (if TransitionMatrix was specified)
             if self.TransitionMatrix is not None:
                 for x_ in range(pop_x):
                     for y_ in range(pop_y):
                         for z_ in range(pop_z):
                             ind = self.population[x_, y_, z_]
@@ -614,28 +696,28 @@
                             ] += 1
                             self.curr_size_list[
                                 self.init_label_list.index(old_label)
                             ] -= 1
 
             # after each birth-death cycle:
 
-            # update scores for all individuals (if TransitionMatrix was specified)
+            # update scores for all individuals (if TransitionMatrix present)
             if self.TransitionMatrix is not None:
                 for x_ in range(self.population.shape[0]):
                     for y_ in range(self.population.shape[1]):
                         for z_ in range(self.init_grid.shape[2]):
                             self._UpdateBirthPayoff(x_, y_, z_)
                             self._UpdateDeathPayoff(x_, y_, z_)
                             self._UpdateBirthFitness(x_, y_, z_)
                             self._UpdateDeathFitness(x_, y_, z_)
             # in other case:
             # re-evaluate the payoffs and fitnesses of only
             # the affected neigbours Individuals in the population
             else:
-                # re-evaluate the payoffs and fitnesses of the affected Individuals in the population
+                # re-evaluate payoffs & fitnesses of affected ind in pop
                 indices_list = [
                     ((x - 1) % pop_x, (y - 1) % pop_y, (z - 1) % pop_z),
                     ((x - 1) % pop_x, (y - 1) % pop_y, z % pop_z),
                     ((x - 1) % pop_x, (y - 1) % pop_y, (z + 1) % pop_z),
                     ((x - 1) % pop_x, y % pop_y, (z - 1) % pop_z),
                     ((x - 1) % pop_x, y % pop_y, z % pop_z),
                     ((x - 1) % pop_x, y % pop_y, (z + 1) % pop_z),
@@ -660,30 +742,36 @@
                     ((x + 1) % pop_x, (y + 1) % pop_y, (z - 1) % pop_z),
                     ((x + 1) % pop_x, (y + 1) % pop_y, z % pop_z),
                     ((x + 1) % pop_x, (y + 1) % pop_y, (z + 1) % pop_z),
                 ]
                 for indices in indices_list:
                     self._UpdateBirthPayoff(indices[0], indices[1], indices[2])
                     self._UpdateDeathPayoff(indices[0], indices[1], indices[2])
-                    self._UpdateBirthFitness(indices[0], indices[1], indices[2])
-                    self._UpdateDeathFitness(indices[0], indices[1], indices[2])
+                    self._UpdateBirthFitness(
+                        indices[0], indices[1], indices[2]
+                    )
+                    self._UpdateDeathFitness(
+                        indices[0], indices[1], indices[2]
+                    )
 
             # update the grid
             for x_ in range(self.curr_grid.shape[0]):
                 for y_ in range(self.curr_grid.shape[1]):
                     for z_ in range(self.curr_grid.shape[2]):
-                        self.curr_grid[x_, y_, z_] = self.population[x_, y_, z_].label
+                        self.curr_grid[x_, y_, z_] = self.population[
+                            x_, y_, z_
+                        ].label
 
             # re-evaluate the population Entropy
             self._UpdateEntropy()
 
             # update the log dataframe
-            for l in range(len(self.init_label_list)):
-                label = self.init_label_list[l]
-                log_df.at[g + 1, label + "__size"] = self.curr_size_list[l]
+            for index in range(len(self.init_label_list)):
+                label = self.init_label_list[index]
+                log_df.at[g + 1, label + "__size"] = self.curr_size_list[index]
                 log_df.at[g + 1, "Entropy"] = self.Entropy
 
         return log_df
 
     def PlotSize3D(self, df, path):
         """Plot the sub-populations' sizes after a simulation.
 
@@ -694,15 +782,15 @@
         """
         plt.figure(figsize=(14, 6))
         ax = plt.gca()
         ax.tick_params(width=1)
         for axis in ["top", "bottom", "left", "right"]:
             ax.spines[axis].set_linewidth(1)
         cmap = plt.get_cmap("coolwarm")
-        columns = [l + "__size" for l in self.init_label_list]
+        columns = [label + "__size" for label in self.init_label_list]
         df_copy = df[columns].copy()
         df_copy.columns = self.init_label_list
         df_copy.plot(linewidth=1.5, ax=ax, cmap=cmap)
         population_size = self.population.size
         ax.set_ylim([0, population_size])
         plt.xlabel("Generation", size=14)
         plt.ylabel("# Individuals", size=14)
@@ -719,13 +807,15 @@
 
         """
         plt.figure(figsize=(14, 6))
         ax = plt.gca()
         ax.tick_params(width=1)
         for axis in ["top", "bottom", "left", "right"]:
             ax.spines[axis].set_linewidth(1)
-        df["Entropy"].plot(color="black", linewidth=1.5, ax=ax, label="Entropy")
+        df["Entropy"].plot(
+            color="black", linewidth=1.5, ax=ax, label="Entropy"
+        )
         plt.xlabel("Generation", size=14)
         plt.ylabel("", size=14)
         ax.tick_params(axis="both", which="major", labelsize=12)
         ax.legend(loc=4, fontsize=20)
         plt.savefig(fname=path, dpi=300)
```

### Comparing `moranpycess-1.0.39/moranpycess/__init__.py` & `moranpycess-1.1.0/moranpycess/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,20 @@
-"""
+""".
+
 ##############################################################################
 #
 #   Init file for the package
 #
 #   AUTHOR: Maciej_Bak
 #   AFFILIATION: University_of_Basel
 #   AFFILIATION: Swiss_Institute_of_Bioinformatics
 #   CONTACT: wsciekly.maciek@gmail.com
 #   CREATED: 20-07-2020
 #   LICENSE: MIT
 #
 ##############################################################################
 """
 
-# imports
-import os
-import sys
-
-# modify PYTHONPATH so that modules can import each other
-sys.path.append(os.path.dirname(os.path.realpath(__file__)))
-
 # import distinct classes from modules of this package
-from .MoranProcess import MoranProcess
-from .MoranProcess2D import MoranProcess2D
-from .MoranProcess3D import MoranProcess3D
+from .MoranProcess import MoranProcess  # noqa
+from .MoranProcess2D import MoranProcess2D  # noqa
+from .MoranProcess3D import MoranProcess3D  # noqa
```

### Comparing `moranpycess-1.0.39/moranpycess.egg-info/PKG-INFO` & `moranpycess-1.1.0/moranpycess.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: moranpycess
-Version: 1.0.39
+Version: 1.1.0
 Summary: Python framework for Moran Processes driven by game theory
-Home-page: https://github.com/AngryMaciek/angry-moran-simulator
-Author: Maciek Bak
-Author-email: wsciekly.maciek@gmail.com
+Author-email: Maciek Bak <wsciekly.maciek@gmail.com>
 License: MIT
-Platform: UNKNOWN
+Project-URL: homepage, https://angrymaciek.github.io/angry-moran-simulator/_build/html/index.html
+Project-URL: repository, https://github.com/AngryMaciek/angry-moran-simulator
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 The following package presents a general game-theoretical framework to carry out scientific simulations according to the Moran model. Registering distinct types of individuals together with specification of payoffs between them allows to replicate evolution of the population and observe growth dynamics.
 
 For more information please visit project's homepage!
-
```

